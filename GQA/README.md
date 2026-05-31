# GQA Knowledge Gap (KG) Annotations

This folder contains Knowledge Gap (KG) annotations for the **GQA** dataset as part of the TinyKGI framework presented in:

**Identifying Knowledge Gaps on the Edge for Visual Question Answering**

## Files

- **TRAIN_QUESTIONS_WITH_KGS.json**
- **VAL_QUESTIONS_WITH_KGS.json**

## Description

These files extend the original GQA dataset with Knowledge Gap (KG) annotations.

Each question entry contains the original GQA metadata together with the additional field:

- **Knowledge_Gaps**: List of Knowledge Gap categories associated with the question.
### Example
```json
{
  "13831865": {
    "question": "Who is walking?",
    "imageId": "2355250",
    "answer": "people",
    "Knowledge_Gaps": ["Activity"]
  }
}
```
## Knowledge Gap Categories
GQA KG labels include:
- Activity
- Attribute
- Direction
- Entity Resolution
- Location
- Material
- Reasoning
- Sentiment
- Size
- State
## Original Dataset
The original GQA dataset is publicly available at:
https://cs.stanford.edu/people/dorarad/gqa/
