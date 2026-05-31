# TinyKGI-KG-Annotations
Knowledge Gap annotations for GQA and CLEVR used in TinyKGI.

# TinyKGI Knowledge Gap (KG) Annotations

This repository contains the Knowledge Gap (KG) annotations developed for the paper:

**Identifying Knowledge Gaps on the Edge for Visual Question Answering**

## Overview

TinyKGI is a lightweight framework for identifying plausible cognitive capabilities that an AI model may lack, referred to as **Knowledge Gaps (KGs)**. These annotations were created to support research on Knowledge Gap Identification for Visual Question Answering (VQA) systems.

The repository provides KG annotations for the following datasets:

- **GQA**
- **CLEVR**

For the **TDIUC** dataset, the original question types are used as Knowledge Gap labels and therefore no additional annotation files are released.

## Repository Structure

```text
gqa/
├── TRAIN_QUESTIONS_WITH_KGS.json
├── VAL_QUESTIONS_WITH_KGS.json
└── README.md
clevr/
├── TRAIN_QUESTIONS_WITH_KGS.json
├── VAL_QUESTIONS_WITH_KGS.json
└── README.md
```

## Annotation Format

The released files extend the original dataset annotations with an additional field:

- **Knowledge_Gaps**: List of Knowledge Gap categories associated with the question.
Example:
```json
{
  "question": "Who is walking?",
  "answer": "people",
  "Knowledge_Gaps": ["Activity"]
}
```
## Knowledge Gap Categories
Examples of KG categories include:
- Activity
- Attribute
- Color
- Counting
- Entity Resolution
- Location
- Material
- Scene Recognition
- Sentiment
- Size
- State
- Utility Affordance
## Original Datasets
The KG annotations provided in this repository are derived from publicly available datasets.
### GQA
https://cs.stanford.edu/people/dorarad/gqa/
### CLEVR
https://cs.stanford.edu/people/jcjohns/clevr/
### TDIUC
https://kushalkafle.com/projects/tdiuc.html
