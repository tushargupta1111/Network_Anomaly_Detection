# Network-Amonaly-Detection

## Project Overview
The primary aim of this project is to enhance the performance of an intrusion detection system using the **XGBoost classifier** through parameter tuning. This project leverages the **CSE-CIC-IDS 2018 dataset**, a widely used benchmark in the cybersecurity domain, to detect and classify network intrusions. Techniques such as **Grid Search** and **Random Search** are employed to optimize hyperparameters and improve performance metrics like accuracy, precision, recall, F1-score, Cohen's Kappa coefficient (CKC), prediction time, and false alarm rate (FAR).

## Dataset Description
We use the **CSE-CIC-IDS 2018 dataset** by the **Canadian Institute for Cybersecurity (CIC)**. This dataset consists of network traffic logs categorized as benign or malicious across 15 classes of attacks. The following pre-processing steps were applied to the raw dataset:
- Encoding of class labels
- Replacing invalid string values (e.g., `inf`, `Infinity`) 
- One-hot encoding of categorical attributes
- Removal of redundant headers
- Reduction of dataset size (~6.3GB to ~1.3GB)
- Stratified random split of data (80% training, 20% validation)
## Dataset Link 
   ```bash
  https://www.kaggle.com/datasets/solarmainframe/ids-intrusion-csv
```

The final processed dataset is stored in an Amazon S3 bucket for training purposes.

## Project Objectives
- **Optimize** the performance of the **XGBoost classifier** algorithm through systematic parameter tuning.
- **Evaluate** the model on the CICIDS 2018 dataset using metrics such as accuracy, precision, recall, F1-score, CKC, and FAR.
- **Explore** the hyperparameter space using **Grid Search** and **Random Search** to find the optimal configuration.
- **Document** and report the findings, methodology, and potential improvements for future research.

## Methodology
1. **XGBoost Classifier**  
   XGBoost is a gradient boosting algorithm known for its speed and performance, particularly for classification tasks.
   
2. **Parameter Tuning**  
   - **Grid Search:** Exhaustive search over predefined parameter grids.
   - **Random Search:** Randomly samples parameter combinations for evaluation.

3. **Experimental Setup**
   - **Data Preprocessing:** Handle missing values, encode categorical features, and scale numerical features.
   - **Feature Engineering:** Select and normalize relevant features.
   - **Splitting Data:** Separate the dataset into training and testing sets.
   - **Model Implementation:** Implement the **XGBoost classifier** using the `xgboost` library.
   - **Parameter Tuning:** Use **Grid Search** and **Random Search** to find the optimal hyperparameters.
   - **Evaluation Metrics:** Use accuracy, precision, recall, F1-score, CKC, and FAR to assess model performance.
   - **Visualization:** Graphical plots to compare results across tuning methods.

4. **Results Analysis**
   - Analyze how different hyperparameters affect model performance.
   - Extract insights into model tuning to guide future improvements.

## Expected Outcomes
- **Optimized XGBoost model**: Higher accuracy and robustness compared to default parameters.
- **Improved Generalization**: Better performance on unseen data and a lower false alarm rate.
- **Hyperparameter Insights**: Understanding of how hyperparameter tuning affects model performance.

## Conclusion
This project aims to improve the performance of the XGBoost classifier on the **CSE-CIC-IDS 2018 dataset** through systematic parameter tuning. By leveraging **Grid Search** and **Random Search**, the project seeks to find the best hyperparameter configuration that maximizes the model’s predictive capabilities while reducing overfitting. The results will provide insights into the optimization process and its impact on intrusion detection in network traffic.

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/yourusername/Network-Intrusion-Detection.git](https://github.com/tushargupta1111/Network-Intrusion-Detection-using-CSE-CIC-IDS-2018-dataset
