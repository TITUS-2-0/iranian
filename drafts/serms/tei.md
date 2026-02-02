

### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Fragment | `div@fragment` | Automatically translated into named div |
| Part | `div@part` | Automatically translated into named div |
| Manuscript | `div@manuscript` | Automatically translated into named div |
| Part of Ms. | `manuscript-part` |  |
| Page of Ms. | `pb@manuscript` |  |
| Line of Ms. | `lb@manuscript` |  |

### Structural overview
```text
text (@xml:lang=xmn-Latn-x-tld)
  body
    div (@data-level=1, @n, @type=fragment, @xml:id) (multiple)
      head (@xml:lang=deu-Latn) (multiple)
      div (@data-level=2, @n, @type=manuscript, @xml:id) (multiple)
        div (@data-level=3, @n, @type=manuscript-part, @xml:id) (multiple)
          p (@xml:id) (multiple)
            [lb (@type=manuscript) (multiple)]
          [pb (@type=recto) (multiple)]
        div (@data-level=3, @n, @type=manuscript-part, @xml:id) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id, @xml:lang=pal-Latn-x-tld) (multiple)
        p (@xml:id) (multiple)
          [note (@xml:id)]
            [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld) (multiple)]
        div (@data-level=3, @n, @type=manuscript, @xml:id) (multiple)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id) (multiple)
            p (@xml:id) (multiple)
              [pb (@n, @type=recto | verso) (multiple)]
              [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
              [note (@xml:id) (multiple)]
                [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld | pal-Latn-x-txl) (multiple)]
              [lb (@n, @type=manuscript) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id, @xml:lang=pal-Latn-x-tld) (multiple)
        div (@data-level=3, @n, @type=manuscript, @xml:id) (multiple)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id) (multiple)
            p (@xml:id) (multiple)
              [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld) (multiple)]
                [lb (@n, @type=manuscript) (multiple)]
                [pb (@n, @type=verso)]
              [lb (@type=manuscript) (multiple)]
            [pb (@type=recto) (multiple)]
        div (@data-level=3, @n, @type=manuscript, @xml:id, @xml:lang=pal-Latn-x-tld)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id)
            p (@xml:id)
              [pb (@n, @type=recto)]
              [lb (@n, @type=manuscript) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id, @xml:lang=sog-Latn) (multiple)
        p (@xml:id) (multiple)
          [pb (@n, @type=recto) (multiple)]
          [lb (@n, @type=manuscript) (multiple)]
          [note (@xml:id) (multiple)]
            [foreign (@xml:lang=deu-Latn | sog-Latn) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [lb (@n, @type=manuscript) (multiple)]
          [note (@xml:id) (multiple)]
            [foreign (@xml:lang=deu-Latn) (multiple)]
          [foreign (@xml:lang=deu-Latn)]
        [pb (@n, @type=recto) (multiple)]
    div (@data-level=1, @n, @type=fragment, @xml:id) (multiple)
      div (@data-level=2, @n, @type=manuscript, @xml:id) (multiple)
        div (@data-level=3, @n, @type=manuscript-part, @xml:id) (multiple)
          p (@xml:id) (multiple)
            [lb (@type=manuscript) (multiple)]
          [pb (@type=recto) (multiple)]
        div (@data-level=3, @n, @type=manuscript-part, @xml:id) (multiple)
      div (@data-level=2, @n, @type=part, @xml:id, @xml:lang=pal-Latn-x-tld) (multiple)
        p (@xml:id) (multiple)
          [note (@xml:id) (multiple)]
            [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld | pal-Latn-x-txl) (multiple)]
          [note (@xml:id, @xml:lang=deu-Latn | pal-Latn-x-tld) (multiple)]
        div (@data-level=3, @n, @type=manuscript, @xml:id) (multiple)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id) (multiple)
            p (@xml:id) (multiple)
              [lb (@n, @type=manuscript) (multiple)]
              [note (@xml:id) (multiple)]
                [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld | pal-Latn-x-txl) (multiple)]
              [note (@xml:id, @xml:lang=deu-Latn) (multiple)]
              [pb (@n, @type=recto | verso) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id, @xml:lang=pal-Latn-x-tld) (multiple)
        div (@data-level=3, @n, @type=manuscript, @xml:id, @xml:lang=pal-Latn-x-tld) (multiple)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id) (multiple)
            p (@xml:id) (multiple)
              [pb (@n, @type=recto | verso) (multiple)]
              [lb (@n, @type=manuscript) (multiple)]
              [note (@xml:id) (multiple)]
                [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld) (multiple)]
        div (@data-level=3, @n, @type=manuscript, @xml:id) (multiple)
          div (@data-level=4, @n, @type=manuscript-part, @xml:id) (multiple)
            p (@xml:id) (multiple)
              [lb (@type=manuscript) (multiple)]
              [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld) (multiple)]
                [lb (@n, @type=manuscript) (multiple)]
            [pb (@type=recto) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id, @xml:lang=pal-Latn-x-tld | sog-Latn) (multiple)
        p (@xml:id) (multiple)
          [lb (@n, @type=manuscript) (multiple)]
          [pb (@n, @type=recto | verso) (multiple)]
          [note (@xml:id) (multiple)]
            [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld | sog-Latn) (multiple)]
          [note (@xml:id, @xml:lang=deu-Latn | sog-Latn) (multiple)]
      div (@data-level=2, @n, @type=part, @xml:id) (multiple)
        p (@xml:id) (multiple)
          [foreign (@xml:lang=deu-Latn | oui-Latn-x-manich-tld | pal-Latn-x-tld | sog-Latn | xmn-Latn-x-txl) (multiple)]
            [lb (@n, @type=manuscript) (multiple)]
            [pb (@n, @type=recto) (multiple)]
            [note (@xml:id) (multiple)]
              [foreign (@xml:lang=deu-Latn | pal-Latn-x-tld | sog-Latn | xmn-Latn-x-txl) (multiple)]
          [pb (@n, @type=recto | verso) (multiple)]
          [lb (@n, @type=manuscript, @xml:lang=oui-Latn-x-manich-tld) (multiple)]
          [note (@xml:id, @xml:lang=deu-Latn)]
          [note (@xml:id)]
            [foreign (@xml:lang=deu-Latn | oui-Latn-x-manich-tld | xmn-Latn-x-txl) (multiple)]
          [lb (@n, @type=manuscript)]
      div (@data-level=2, @n, @type=manuscript, @xml:id, @xml:lang=deu-Latn)
        div (@data-level=3, @n, @type=manuscript-part, @xml:id)
          p (@xml:id)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="H" xml:id="fragment-1" type="fragment" data-level="1">
				<head xml:lang="deu-Latn">Die Überschriften des parthischen und des soghdischen Textes</head>
				<div n="1" xml:id="fragment-1-manuscript-1" type="manuscript" data-level="2">
					<div n="1" xml:id="fragment-1-manuscript-1-manuscript-part-1" type="manuscript-part" data-level="3">
						<pb type="recto"/>
						<p xml:id="fragment-1-manuscript-1-manuscript-part-1-p-1">
							<lb type="manuscript"/>
						</p>
					</div>
				</div>
				<div n="1" xml:id="fragment-1-part-1" type="part" data-level="2" xml:lang="pal-Latn-x-tld">
					<p xml:id="fragment-1-part-1-p-2">gy՚n<note xml:id="fragment-1-part-1-p-2-note-1">
  ...
```
