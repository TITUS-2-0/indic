# Dataset 'ys'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ind/aind/ved/yvw/dhs/ys/ys.htm).

* URL: https://github.com/TITUS-2-0/indic/tree/main/drafts/ys/
* version: unreleased
* date: 2025-04-08

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/indic/tree/main/drafts/ys/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Paragraph | `div@paragraph` | Automatically translated into named div |
| Verse | `lg@stanza` |  |
| Halfverse | `l` |  |

### Structural overview
```text
text (@xml:lang=san-Latn-x-vedic-prose-unacc-tld)
  front (@xml:id)
    titlePage (@xml:id)
      docTitle (@xml:id)
        titlePart (@xml:id) (multiple)
  body
    div (@data-level=1, @n, @type=chapter, @xml:id) (multiple)
      head (@xml:lang=san-Latn-x-vedic-prose-unacc-txl) (multiple)
      div (@data-level=2, @n, @type=paragraph, @xml:id) (multiple)
        head (@xml:lang=san-Latn-x-vedic-prose-unacc-txl) (multiple)
        lg (@n, @type=stanza, @xml:id) (multiple)
          l (@n, @xml:id) (multiple)
            [foreign (@xml:lang=eng-Latn | san-Latn-x-vedic-metric-unacc-txl | san-Latn-x-vedic-prose-unacc-txl) (multiple)]
            [pb (@n) (multiple)]
      [pb (@n) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="chapter-1" type="chapter" data-level="1">
				<pb n="1"/>
				<head xml:lang="san-Latn-x-vedic-prose-unacc-txl">ācāra-adʰyāya</head>
				<div n="1" xml:id="chapter-1-paragraph-1" type="paragraph" data-level="2">
					<head xml:lang="san-Latn-x-vedic-prose-unacc-txl">upodgʰāta-prakaraṇam</head>
					<lg n="1" type="stanza" xml:id="chapter-1-paragraph-1-lg-1">
						<l n="a" xml:id="chapter-1-paragraph-1-lg-1-l-1">
							<foreign xml:lang="san-Latn-x-vedic-metric-unacc-txl">yogi-īśvaram yājñavalkyam \sampūjya munayo_\abruvan /</foreign>
						</l>
						<l n="c" xml:id="chapter-1-paragraph-1-lg-1-l-2">
							<foreign xml:lang="san-Latn-x-vedic-metric-unacc-txl">varṇa-āśrama-itarāṇām no \brūhi dʰarmān aśeṣataḥ //</foreign>
						</l>
  ...
```
