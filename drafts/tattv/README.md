# Dataset 'tattv'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ind/aind/jskt/tattvs/tattv.htm).

* URL: https://github.com/TITUS-2-0/indic/tree/main/drafts/tattv/
* version: unreleased
* date: 2025-04-08

## Citation
```text
Digital version of [Untitled Dataset] (draft version). In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://github.com/TITUS-2-0/indic/tree/main/drafts/tattv/, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Adhyaya | `div@adhyaya` | Automatically translated into named div |
| Sentence | `s` |  |

### Structural overview
```text
text (@xml:lang=san-Latn-x-classic-unacced-tld)
  body
    div (@data-level=1, @n, @type=adhyaya, @xml:id) (multiple)
      p (@xml:id) (multiple)
        s (@n, @xml:id) (multiple)
          [note (@xml:id, @xml:lang=eng-Latn) (multiple)]
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="1" xml:id="adhyaya-1" type="adhyaya" data-level="1">
				<p xml:id="adhyaya-1-p-1">
					<s n="1" xml:id="adhyaya-1-p-1-s-1">samyagdarśana jñāna cāritrāṇi mokṣamārgaḥ</s>
					<s n="2" xml:id="adhyaya-1-p-1-s-2">tattvārthaśraddhānaṃ samyagdarśanam</s>
					<s n="3" xml:id="adhyaya-1-p-1-s-3">tan nisargād adhigamād vā</s>
					<s n="4" xml:id="adhyaya-1-p-1-s-4">jīvājīvāsrava bandha saṃvara nirjarā mokṣāstattvaṃ</s>
					<s n="5" xml:id="adhyaya-1-p-1-s-5">nāma sthāpanā dravya bhāvatastannyāsaḥ</s>
					<s n="6" xml:id="adhyaya-1-p-1-s-6">pramāṇanayair adhigamaḥ</s>
					<s n="7" xml:id="adhyaya-1-p-1-s-7">nirdeśa svāmitva sādhana adhikaraṇa sthiti vidhānataḥ</s>
					<s n="8" xml:id="adhyaya-1-p-1-s-8">sat saṃkhyā kṣetra sparśana kālāntara bhāvālpa bahuttvaiśca</s>
					<s n="9" xml:id="adhyaya-1-p-1-s-9">matiśrutāvadhimanaḥ paryaya kevalāni jñānam</s>
					<s n="10" xml:id="adhyaya-1-p-1-s-10">tat pramāṇe</s>
  ...
```
