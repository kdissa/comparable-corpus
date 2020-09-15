## Comparable Sentences with Golden Alignment

This repository contains 12 comparable corpora for Sinhala - English, Tamil - English and Sinhala - Tamil language pairs with ground truth alignments which can be used to evaluate sentence alignment systems.
Under each language pair there are 4 datasets containing documents collected from 4 diffrenet news websites.
Each such dataset contains two monolingual corpora of about 1521 - 4898 sentence splitted documents.
For each document in one language, its comparable document is stored with the same name under the other language folder.

Sentence splitting for each language is done using the following tokenizers,
* Sinhala - [https://github.com/ysenarath/sinling](https://github.com/ysenarath/sinling)
* English - [https://pypi.org/project/sentence-splitter/](https://pypi.org/project/sentence-splitter/)
* Tamil - [https://github.com/AshokR/TamilNLP](https://github.com/AshokR/TamilNLP)

Sentence splitting output of the tokenizers and a human being is not 100% equivalent.
To remove the impact of this in the final results, ground truth sentence alignment was done using the sentence splitted documents as the input to the huan annotator.

Each sentence in documents is tagged with an id and those ids are included in the ground truth alignment instead of the actual sentences.

## Folder structure

```.
├── Sinhala - English
│   ├── Army_News
│   │   ├── Sinhala
│   │   ├── English
│   │   └── Armynews.si-en
│   ├── Hiru
│   │   ├── Sinhala
│   │   ├── English
│   │   └── Hiru.si-en
│   ├── ITN
│   │   ├── Sinhala
│   │   ├── English
│   │   └── ITN.si-en
│   └── Newsfirst
│       ├── Sinhala
│       ├── English
│       └── Newsfirst.si-en
├── Tamil - English
│   ├── ArmyNews
│   │   ├── Tamil
│   │   ├── English
│   │   └── Armynews.ta-en
│   ├── Hiru
│   │   ├── Tamil
│   │   ├── English
│   │   └── Hiru.ta-en
│   ├── ITN
│   │   ├── Tamil
│   │   ├── English
│   │   └── ITN.ta-en
│   └── Newsfirst
│       ├── Tamil
│       ├── English
│       └── Newsfirst.ta-en
└── Sinhala - Tamil
    ├── ArmyNews
    │   ├── Tamil
    │   ├── Sinhala
    │   └── Armynews.si-ta
    ├── Hiru
    │   ├── Tamil
    │   ├── Sinhala
    │   └── Hiru.si-ta
    ├── ITN
    │   ├── Tamil
    │   ├── Sinhala
    │   └── ITN.si-ta
    └── Newsfirst
        ├── Tamil
        ├── Sinhala
        └── Newsfirst.si-ta
 ```
