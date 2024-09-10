# Foetal Health Prediction using Machine Learning

## Overview

This project aims to predict foetal health using machine learning algorithms applied to Cardiotocography (CTG) data. The system classifies the foetal health into three categories: **Normal**, **Suspect**, and **Pathological**. The goal is to assist medical professionals in making more accurate decisions, thereby improving outcomes and reducing potential risks.

## Dataset

The dataset used for this project includes features extracted from CTG data such as:
- Baseline value
- Accelerations
- Foetal movement
- Uterine contraction
- Decelerations, etc.

## Data Preprocessing

1. **Handling Missing Data**: Any missing values were imputed using the K-Nearest Neighbors (KNN) algorithm.
2. **Outlier Removal**: Boxplots were used to detect and replace outliers with appropriate values.
3. **Feature Engineering**: Features with high correlation were removed to reduce redundancy and improve model performance.

## Models Used

The following machine learning models were trained and evaluated:
- **Logistic Regression**: Achieved an accuracy of 74.66%.
- **Naive Bayes**: Achieved an F1 score of 66.71%.
- **Random Forest**: Achieved an F1 score of 81%.
- **AdaBoost Classifier**: Achieved an F1 score of 75.77%.
- **K-Nearest Neighbors (KNN)**: Achieved an F1 score of 70.47%.
- **Artificial Neural Network (ANN)**: Best performer with an F1 score of 81.20%.
- **Support Vector Machine (SVM)**: Achieved an F1 score of 74.23% using a polynomial kernel.

## Cross-Validation

To ensure robust model performance, 10-fold cross-validation (k=10) was applied, and the **F1 score** was used as the evaluation metric.

## Results

| Model                   | F1 Score  |
|-------------------------|-----------|
| **Artificial Neural Network (ANN)** | **81.20%**   |
| Random Forest            | 81.00%    |
| AdaBoost                 | 75.77%    |
| Logistic Regression      | 74.66%    |
| Support Vector Machine   | 74.23%    |
| K-Nearest Neighbors      | 70.47%    |
| Naive Bayes              | 66.71%    |

## Conclusion

- **Artificial Neural Network (ANN)** provided the best performance in predicting foetal health with an F1 score of 81.20%.
- Machine learning models can help in diagnosing potential risks more accurately, aiding healthcare professionals in decision-making.

## How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Foetal-Health-Prediction-ML-Project.git
    ```
2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Jupyter notebook:
    ```bash
    jupyter notebook Foetal_Health_Prediction.ipynb
    ```

## Contributors

- Anupam Garg ([anupam20555@iiitd.ac.in](mailto:anupam20555@iiitd.ac.in))
- Bhavya Jain ([bhavya20428@iiitd.ac.in](mailto:bhavya20428@iiitd.ac.in))
- Shivam Kumar Jha ([shivam20332@iiitd.ac.in](mailto:shivam20332@iiitd.ac.in))
- Subhanshu Bansal ([subhanshu20135@iiitd.ac.in](mailto:subhanshu20135@iiitd.ac.in))

## License

This project is licensed under the MIT License - see the LICENSE file for details.

