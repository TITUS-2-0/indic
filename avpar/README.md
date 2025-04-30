# Dataset 'Atharva-Veda: Atharvaveda-Pariśiṣṭas'

![Static Badge](https://img.shields.io/badge/TEI_validation-passing-green)

This is a TEI port of a [TITUS dataset](http://titus.uni-frankfurt.de/texte/etcs/ind/aind/ved/av/avparis/avpar.htm).

* URL: https://titus2.uni-frankfurt.de/dataset/avpar
* version: 0.1.0
* date: 2025-04-23

## Citation
```text
Digital version of Atharva-Veda: Atharvaveda-Pariśiṣṭas (v0.1.0). By: Jost Gippert, Arlo Griffiths, Yuri Ishii, Florian Matter. In: Carling, Gerd & Jost Gippert (2025). TITUS 2.0. Frankfurt: Goethe University. (URL: https://titus2.uni-frankfurt.de/dataset/avpar, visited on <insert date>)
```

## TEI encoding


### Unit Mapping
The TITUS 1 structural units are mapped onto TEI as follows:

| Source Unit | TEI Mapping | Notes |
|-------------|-------------|-------|
| Parisista | `div@parisista` | Automatically translated into named div |
| Section | `div@section` | Automatically translated into named div |
| Verse | `ab@verse` |  |

### Structural overview
```text
text (@xml:lang=san-Latn-x-vedic-prose-unacc-tld)
  body
    div (@data-level=1, @n, @type=pariśiṣṭa, @xml:id) (multiple)
      div (@data-level=2, @n, @type=section, @xml:id)
        ab (@n, @type=verse, @xml:id)
```

### Structure Example

```xml
<div xmlns="http://www.tei-c.org/ns/1.0" n="0" xml:id="pari&#x15B;i&#x1E63;&#x1E6D;a-1" type="pari&#x15B;i&#x1E63;&#x1E6D;a" data-level="1">
				<div n="0" xml:id="pariśiṣṭa-1-section-1" type="section" data-level="2">
					<ab n="0" type="verse" xml:id="pariśiṣṭa-1-section-1-ab-1">śrīgaṇeśāya namaḥ || oṃ namo 'tʰarvātmane vāmadevāya śivāya || śrīsarasvatyai namaḥ ||</ab>
				</div>
			</div>
```
