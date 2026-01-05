# Model Card: Breast Cancer Detection Classifier

## Model Details

- **Model Name**: Breast Cancer Logistic Regression Classifier
- **Version**: 1.0
- **Model Type**: Binary Classification
- **Algorithm**: Logistic Regression
- **Framework**: scikit-learn

## Intended Use

### Primary Use Case

- **Purpose**: Classify breast tumors as Malignant or Benign based on cell nuclei features
- **Intended Users**: Healthcare researchers, data scientists, educational purposes
- **Out of Scope**: This model should NOT be used as a sole diagnostic tool in clinical settings

### Limitations

- Model is trained on a specific dataset and may not generalize to all populations
- Should be used as a decision support tool, not a replacement for medical professionals
- Performance may vary with different imaging equipment or techniques

## Training Data

### Dataset

- **Source**: Wisconsin Breast Cancer Dataset (UCI Machine Learning Repository)
- **Size**: 569 samples
- **Class Distribution**:
  - Benign: 357 (62.7%)
  - Malignant: 212 (37.3%)

### Features

- 30 numerical features computed from cell nuclei images
- Features include: radius, texture, perimeter, area, smoothness, etc.

### Preprocessing

1. Dropped irrelevant columns (id, Unnamed: 32)
2. Label encoding (M=1, B=0)
3. Stratified train-test split (80/20)
4. StandardScaler normalization

## Evaluation Results

### Test Set Performance (n=114)

| Metric                | Value  |
| --------------------- | ------ |
| Accuracy              | 96.49% |
| Precision (Benign)    | 0.96   |
| Recall (Benign)       | 0.99   |
| Precision (Malignant) | 0.97   |
| Recall (Malignant)    | 0.93   |

### Confusion Matrix

```
              Predicted
              B     M
Actual  B   [71     1]
        M   [ 3    39]
```

## Ethical Considerations

- **Bias**: Model trained on data primarily from Wisconsin, may not represent global diversity
- **False Negatives**: 3 malignant cases were misclassified as benign (potentially serious)
- **Transparency**: Model coefficients can be inspected for feature importance
- **Privacy**: Original patient IDs are not used in the model

## Recommendations

1. Use as a screening support tool only
2. Always consult medical professionals for diagnosis
3. Consider ensemble methods for improved accuracy
4. Regular model updates with new data recommended
