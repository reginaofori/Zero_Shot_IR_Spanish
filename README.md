## A Zero-Shot Monolingual Dual Stage Information Retrieval System for Spanish Biomedical Systematic Literature Reviews (Accepted into NAACL 2024 Main Conference)

### Table of Contents
- [Abstract](#features)
- [Methodology](#installation)
- [Prerequisites](#usage)
- [Spanish SR Train/Test Dataset](#visualizing-attacks)
- [Models](#generating-adversarial-images)
- [Limitation](#limitation)


### Abstract

Systematic Reviews (SRs) are foundational in healthcare for synthesising evidence to inform clinical practices. Traditionally skewed towards English-language databases, SRs often exclude significant research in other languages, leading to potential biases. This study addresses this gap by focusing on Spanish, a language notably underrepresented in SRs. We present a foundational zero-shot dual information retrieval (IR) baseline system, integrating traditional retrieval methods with pre-trained language models and cross-attention re-rankers for enhanced accuracy in Spanish biomedical literature retrieval. Utilising the LILACS database, known for its comprehensive coverage of Latin American and Caribbean biomedical literature, we evaluate the approach with three real-life case studies in Spanish SRs. The findings demonstrate the system's efficacy and underscore the importance of query formulation. This study contributes to the field of IR by promoting language inclusivity and supports the development of more comprehensive and globally representative healthcare guidelines.

For more details, please check the latest version of the paper


### Methodology

![Image Alt text](dual_encoder_naacl.PNG)


###  Prerequisites
``` bash
- Python 3.6
- sklearn
- spacy
- torch
- transformers
```

### Spanish SR Train/Test Dataset

- Training Dataset: Spanish abstracts from 2009 to 2023 were collected from the [LILACS](https://lilacs.bvsalud.org/en/) database. To obtain abstract-queries pair for training, the titles of biomedical abstracts indexed and collected from the [LILACS](https://lilacs.bvsalud.org/en/) database were converted into questions/queries.


- Testing Dataset: To evaluate the performance of the investigated model, we used three biomedical human annotated Spanish SR case studies: **SB**: [Oral health and obesity in Mexico (salud bucal y obesidad en México)](https://academic.oup.com/nutritionreviews/article/80/6/1694/6402007?login=false), **SM**: [Mental health and obesity in Mexico (salud mental y obesidad en México)](https://academic.oup.com/nutritionreviews/article/81/6/658/6717764?login=false), and **PO**: [Obesity prevention in Mexican children (prevención de obesidad en ninos mexicanos)](https://link.springer.com/article/10.1007/s11121-021-01316-6).







