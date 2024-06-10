## Summary

This report presents an analysis of a housing dataset using various Support Vector Machine (SVM) models to predict home ownership (owner-occupied or renter-occupied). The key findings are:

1. **Feature Importance**: Permutation feature importance revealed that 'BEDROOMS', 'AGE', 'COSTWATR', 'ROOMS', and 'DENSITY' were the most significant features for predicting home ownership across all SVM models.[1]

2. **Linear SVM**: The linear SVM achieved an accuracy of 84.04% using the top 5 features. However, using only the top 2 features ('BEDROOMS' and 'AGE') resulted in a lower accuracy of 81.19%.[1]

3. **Radial (RBF) SVM**: The RBF SVM emerged as the best model, achieving the highest accuracy of 85.59% with the optimal parameter combination. It outperformed the linear and polynomial SVMs, demonstrating its ability to capture complex, non-linear relationships in the dataset.[1]

4. **Confusion Matrices**: The confusion matrices revealed that while the models performed well in correctly classifying instances, there were still a considerable number of false positives and false negatives, indicating room for improvement in distinguishing between classes.[1]

5. **Decision Boundary**: The decision boundary plot for the RBF SVM with the top 2 features ('COSTWATR' and 'BEDROOMS') visually illustrates how the model separates the two classes based on these features.[1]

Overall, the analysis highlights the effectiveness of SVM models, particularly the RBF kernel, in predicting home ownership based on demographic factors. The report also emphasizes the importance of feature selection and parameter tuning for optimal model performance.
