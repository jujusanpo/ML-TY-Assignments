# Model Performance Comparison: SVM vs Decision Tree

This report compares the performance of **Support Vector Machine (SVM)** and **Decision Tree** models applied to the Cleveland Heart Disease dataset.

## 1. Support Vector Machine (SVM)

- **Accuracy**: 80.22%
- **Classification Report**:

| Class   | Precision | Recall | F1-Score |
|---------|-----------|--------|----------|
| False   | 0.79      | 0.86   | 0.82     |
| True    | 0.82      | 0.74   | 0.78     |

- **Accuracy**: 80.22%  
- **Macro Average**: Precision: 0.80, Recall: 0.80, F1-Score: 0.80  
- **Weighted Average**: Precision: 0.80, Recall: 0.80, F1-Score: 0.80

### Key Insights:
- The SVM model achieves an accuracy of 80.22%, with solid recall for the "False" class (0.86), but slightly lower recall for the "True" class (0.74). This suggests that the model is better at identifying individuals without heart disease.

## 2. Decision Tree

- **Accuracy**: 78.33%
- **Classification Report**:

| Class   | Precision | Recall | F1-Score |
|---------|-----------|--------|----------|
| 0       | 0.87      | 0.75   | 0.81     |
| 1       | 0.69      | 0.83   | 0.75     |

- **Accuracy**: 78.33%  
- **Macro Average**: Precision: 0.78, Recall: 0.79, F1-Score: 0.78  
- **Weighted Average**: Precision: 0.80, Recall: 0.78, F1-Score: 0.79

### Key Insights:
- The Decision Tree model achieves an accuracy of 78.33%. While its precision for the "False" class is high (0.87), its recall for the "True" class is quite strong (0.83), indicating that the model is more effective at identifying individuals with heart disease than the SVM model.

## 3. Summary and Conclusion

- **SVM** provides slightly higher overall accuracy (80.22%) compared to the Decision Tree (78.33%).  
- The **SVM** model is more effective in precision for both classes, but its **recall for "True"** (heart disease cases) is slightly lower than the **Decision Tree**, which has better recall for the positive class.  
- **Decision Tree** offers a good balance in recall for the "True" class (heart disease cases), making it more suitable when the goal is to minimize missed heart disease predictions. 

### Conclusion:
In conclusion, the SVM model performs better in terms of overall accuracy, but the Decision Tree model might be more preferable if the goal is to reduce false negatives (missed heart disease cases).
