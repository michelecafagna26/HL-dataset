# The High-Level Dataset

The High-Level (HL) dataset aligns object-centric descriptions from COCO with high-level descriptions crowdsourced along 3 axes: scene, action, rationale

The HL dataset contains 149997 images from COCO and a total of 134973 crowdsourced captions (3 captions for each axis) aligned with ~749984 object-centric captions from COCO.

Each axis is collected by asking the following 3 questions:

- Where is the picture taken?
- What is the subject doing?
- Why is the subject doing it?

The high-level descriptions capture the human interpretations of the images. These interpretations contain abstract concepts not directly linked to physical objects. Each high-level description is provided with a confidence score, crowdsourced by an independent worker measuring the extent to which the high-level description is likely given the corresponding image, question, and caption. The higher the score, the more the high-level caption can is close to commonsense (in a Likert scale from 1-5).

---
## Quick start 

### Huggingface Hub

This dataset is available on Huggingface Hub: [```michelecafagna26/hl```](https://huggingface.co/datasets/michelecafagna26/hl)

You can use it directly in the ```datasets``` library:

```python
from datasets import load_dataset

dataset = load_dataset("michelecafagna26/hl")
```

### Clone this repo

You can download the annotations by cloning this repo

```bash
git clone git@github.com:michelecafagna26/hl.git
```

Download and extract the images [here](https://huggingface.co/datasets/michelecafagna26/hl/resolve/main/data/images.tar.gz)

### Languages

All the captions are provided in English

## Dataset Structure

The dataset is provided with images from COCO and two metadata jsonl files containing the annotations

### Data Instances

An instance looks like this:
```json
{
  "file_name": "COCO_train2014_000000138878.jpg",
  "captions": {
    "scene": [
      "in a car",
      "the picture is taken in a car",
      "in an office."
    ],
    "action": [
      "posing for a photo",
      "the person is posing for a photo",
      "he's sitting in an armchair."
    ],
    "rationale": [
      "to have a picture of himself",
      "he wants to share it with his friends",
      "he's working and took a professional photo."
    ],
    "object": [
      "A man sitting in a car while wearing a shirt and tie.",
      "A man in a car wearing a dress shirt and tie.",
      "a man in glasses is wearing a tie",
      "Man sitting in the car seat with button up and tie",
      "A man in glasses and a tie is near a window."
    ]
  },
  "confidence": {
    "scene": [
      5,
      5,
      4
    ],
    "action": [
      5,
      5,
      4
    ],
    "rationale": [
      5,
      5,
      4
    ]
  },
  "purity": {
    "scene": [
      -1.1760284900665283,
      -1.0889461040496826,
      -1.442818284034729
    ],
    "action": [
      -1.0115827322006226,
      -0.5917857885360718,
      -1.6931917667388916
    ],
    "rationale": [
      -1.0546956062316895,
      -0.9740906357765198,
      -1.2204363346099854
    ]
  },
  "diversity": {
    "scene": 25.965358893403383,
    "action": 32.713305568898775,
    "rationale": 2.658757840479801
  }
}
```

### Data Fields

- ```file_name```: original COCO filename
- ```captions```: Dict containing all the captions for the image. Each axis can be accessed with the axis name and it contains a list of captions.
- ```confidence```: Dict containing the captions confidence scores. Each axis can be accessed with the axis name and it contains a list of captions. Confidence scores are not provided for the _object_ axis (COCO captions).t
- ```purity score```: Dict containing the captions purity scores. The purity  score measures the semantic similarity of the captions within the same axis (Bleurt-based).
- ```diversity score```: Dict containing the captions diversity scores. The diversity  score measures the lexical diversity of the captions within the same axis (Self-BLEU-based).

### Data Splits

There are 14997 images and 134973 high-level captions split into:
- Train-val: 13498 images and 121482 high-level captions
- Test: 1499 images and 13491 high-level captions

### Dataset Curators

Michele Cafagna

---

### Licensing Information

The Images and the object-centric captions follow the [COCO terms of Use](https://cocodataset.org/#termsofuse)
The remaining annotations are licensed under Apache-2.0 license.

### Citation Information

```
```
