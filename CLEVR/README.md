# CLEVR Knowledge Gap (KG) Annotations

This folder contains Knowledge Gap (KG) annotations for the **CLEVR** dataset as part of the TinyKGI framework presented in:

**Identifying Knowledge Gaps on the Edge for Visual Question Answering**

## Files

- **TRAIN_QUESTIONS_WITH_KGS.json**
- **VAL_QUESTIONS_WITH_KGS.json**

## Description

These files extend the original CLEVR dataset with Knowledge Gap (KG) annotations.

Each question entry contains the original CLEVR metadata together with the additional field:

- **Knowledge_Gaps**: List of Knowledge Gap categories associated with the question.
### Example
```json
{
  "image_index": 0,
  "question": "Are there any other things that are the same shape as the big metallic object?",
  "answer": "no",
  "Knowledge_Gaps": [
    "Material",
    "EntityResolution",
    "Size",
    "Attribute"
  ]
}
```
## Knowledge Gap Categories
CELVR KG labels include:
- Attribute
- Counting
- Direction
- Entity Resolution
- Material
- Size
## Original Dataset
The original CLEVR dataset is publicly available at:
https://cs.stanford.edu/people/jcjohns/clevr/
