# Dataset 'Sindbad-Name'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etca/iran/niran/npers/sindbad/sindb.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/sindb
* version: unreleased
* date: 2025-04-19

## Citation
```text
Digital version of Sindbad-Name by Aḥmad bin Alī Ẓahīrī Samarqandī (draft version). By: Tamaz Abašidze, Jost Gippert, Florian Matter, Xatuna Todua. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/sindb, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| `Section / Image` (hierarchical) | `section` (hierarchical) |  |
| `Add.` (linear) | `milestone@add` (linear) |  |
| `Page` (hierarchical) | `pb` (linear) |  |
| `Line` (hierarchical) | `lb` (linear) |  |

### Structural overview
```text
text (@xml:lang=pes-Arab-x-persian)
  body (@rend=rtl)
    p (@xml:id)
    div (@data-level=1, @n, @type=section, @xml:id) (multiple)
      p (@xml:id) (multiple)
        [lb (@n) (multiple)]
        [pb (@n) (multiple)]
        [milestone (@n, @unit=add, @xml:id) (multiple)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="section-1" type="section" data-level="1">
        <pb n="31"/>
        <p xml:id="section-1-p-2">
          <lb n="1"/>ابتداى کتاب سندباذ
          <lb n="2"/>چنين گويند راويانِ حديت و خذاوندانِ تاريخ کى در موصيِايّام
          <lb n="3"/>و سوالفِ اعوام در اقليمِ هندوستان ياذشاهى بوذه است کورديس نام کى صحايف
          <lb n="4"/>معالى جهاندارى را بمکارمِ احلاقهِ حميده موسح گردانيذه بوز، ورداى مفاخرِ
          <lb n="5"/>پادشاهى را بمآثرِ اعراقِ کريم مطرّز کرده، و روزگارِ او بجمالِ عدل آراسته
          <lb n="6"/>و اوصافِ و بکمالِ فصل مشهور شذه، دولتى مطاع و حشمتى مطيعم، مدّتى
          <lb n="7"/>طويل و مملکتى عريص، دستِ تناولِ حاسدان و تطاولِ قاصدان از مملکتِ
          <lb n="8"/>او بسته و کوتاه، و چشمِ اطماعِ فاسدهء متعدّيان در دولت او پوشيذه و فراز،
          <lb n="9"/>هميشه مُتابعِ عدل و مطاوعِ عقل بوذى، و آثار و اخبارِ رفتگان و سُنَن وِ و سَِيرِ
  ...
```
