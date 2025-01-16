# Dataset Information

## Primary Sources

1. COCO Dataset (2017)
   - 330K images
   - 80 object categories
   - Person detection focus
   - [Source](https://cocodataset.org/)

2. Custom Motion Dataset
   - 50,000 video frames
   - Motion annotations
   - Indoor/outdoor scenes
   - [Kaggle Link](https://www.kaggle.com/datasets/tensorflow/coco-2017)

## Dataset Statistics
- Total Images: 300,000
- Training: 250,000
- Validation: 25,000
- Test: 25,000

## Class Distribution
```python
classes = {
    'person': 45%,
    'vehicle': 20%,
    'animal': 15%,
    'other': 20%
}
```

## Annotation Format
```json
{
  "image_id": "000000000001",
  "category_id": 1,
  "bbox": [100, 100, 50, 80],
  "motion": true,
  "motion_intensity": 0.85
}
```

## Data Preprocessing
1. Resize: 300x300
2. Normalization: [0,1]
3. Data Augmentation:
   - Random flip
   - Color jitter
   - Motion blur