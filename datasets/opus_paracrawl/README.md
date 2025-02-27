---
annotations_creators:
- found
language_creators:
- found
language:
- bg
- ca
- cs
- da
- de
- el
- en
- es
- et
- eu
- fi
- fr
- ga
- gl
- ha
- hr
- hu
- ig
- is
- it
- km
- lt
- lv
- mt
- my
- nb
- ne
- nl
- nn
- pl
- pt
- ro
- ru
- si
- sk
- sl
- so
- sv
- sw
- tl
license:
- cc0-1.0
multilinguality:
- multilingual
size_categories:
- 100K<n<1M
- 10K<n<100K
- 1M<n<10M
source_datasets:
- original
task_categories:
- translation
task_ids: []
paperswithcode_id: null
pretty_name: OpusParaCrawl
configs:
- de-pl
- el-en
- en-ha
- en-ig
- en-km
- en-so
- en-sw
- en-tl
- es-gl
- fr-nl
---

# Dataset Card for OpusParaCrawl

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks and Leaderboards](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-fields)
  - [Data Splits](#data-splits)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)
  - [Contributions](#contributions)

## Dataset Description

- **Homepage:** http://opus.nlpl.eu/ParaCrawl.php
- **Repository:** None
- **Paper:** http://www.lrec-conf.org/proceedings/lrec2012/pdf/463_Paper.pdf
- **Leaderboard:** [More Information Needed]
- **Point of Contact:** [More Information Needed]

### Dataset Summary

Parallel corpora from Web Crawls collected in the ParaCrawl project.

Tha dataset contains 40 languages and 41 bitexts.

To load a language pair which isn't part of the config, all you need to do is specify the language code as pairs,
e.g.

```python
dataset = load_dataset("opus_paracrawl", lang1="en", lang2="so")
```

You can find the valid pairs in Homepage section of Dataset Description: http://opus.nlpl.eu/ParaCrawl.php

### Supported Tasks and Leaderboards

[More Information Needed]

### Languages

The languages in the dataset are:
- bg
- ca
- cs
- da
- de
- el
- en
- es
- et
- eu
- fi
- fr
- ga
- gl
- ha
- hr
- hu
- ig
- is
- it
- km
- lt
- lv
- mt
- my
- nb
- ne
- nl
- nn
- pl
- pt
- ro
- ru
- si
- sk
- sl
- so
- sv
- sw
- tl

## Dataset Structure

### Data Instances

```
{
  'id': '0', 
  'translation': {
    "el": "Συνεχίστε ευθεία 300 μέτρα μέχρι να καταλήξουμε σε μια σωστή οδός (ul. Gagarina)? Περπατήστε περίπου 300 μέτρα μέχρι να φτάσετε το πρώτο ορθή οδός (ul Khotsa Namsaraeva)?",
    "en": "Go straight 300 meters until you come to a proper street (ul. Gagarina); Walk approximately 300 meters until you reach the first proper street (ul Khotsa Namsaraeva);"
  }
}
```

### Data Fields

- `id` (`str`): Unique identifier of the parallel sentence for the pair of languages.
- `translation` (`dict`): Parallel sentences for the pair of languages.

### Data Splits

The dataset contains a single `train` split.

## Dataset Creation

### Curation Rationale

[More Information Needed]

### Source Data

[More Information Needed]

#### Initial Data Collection and Normalization

[More Information Needed]

#### Who are the source language producers?

[More Information Needed]

### Annotations

[More Information Needed]

#### Annotation process

[More Information Needed]

#### Who are the annotators?

[More Information Needed]

### Personal and Sensitive Information

[More Information Needed]

## Considerations for Using the Data

### Social Impact of Dataset

[More Information Needed]

### Discussion of Biases

[More Information Needed]

### Other Known Limitations

[More Information Needed]

## Additional Information

### Dataset Curators

[More Information Needed]

### Licensing Information

- Creative commons CC0 (no rights reserved)

### Citation Information

```bibtex
@InProceedings{TIEDEMANN12.463,
author = {J{\"o}rg Tiedemann},
title = {Parallel Data, Tools and Interfaces in OPUS},
booktitle = {Proceedings of the Eight International Conference on Language Resources and Evaluation (LREC'12)},
year = {2012},
month = {may},
date = {23-25},
address = {Istanbul, Turkey},
editor = {Nicoletta Calzolari (Conference Chair) and Khalid Choukri and Thierry Declerck and Mehmet Ugur Dogan and Bente Maegaard and Joseph Mariani and Jan Odijk and Stelios Piperidis},
publisher = {European Language Resources Association (ELRA)},
isbn = {978-2-9517408-7-7},
language = {english}
}
```

### Contributions

Thanks to [@rkc007](https://github.com/rkc007) for adding this dataset.
