# Psych-755-final-project

## Project Contributors

- Jessica Tanchone  
- Miao Yu

This project aimed to predict the presence of fatigue, a common somatic symptom, using psychosocial and demographic variables from the publicly available EAMMi2 dataset (Grahe et al., 2018). We conducted exploratory data analysis (EDA) to examine variable distributions, identify outliers, and assess correlations between predictors. We also ran sanity checks to ensure data quality, such as inspecting missingness, checking for class imbalance, and confirming theoretical relevance of predictors. A feedforward neural network was implemented using TensorFlow’s Keras API. The model included an input layer with 24 features, two hidden layers (64 and 32 units) with ReLU activation, dropout layers (rate = 0.3), and a sigmoid output layer for binary classification. The model was trained with the Adam optimizer (learning rate = 0.001), binary cross-entropy loss, and evaluated using accuracy and AUC. The data were split into training (70%) and testing (30%) sets with stratified sampling. StandardScaler was used for normalization, and simple imputation handled missing values. The final model achieved 87.5% accuracy and an AUC of 0.74. While performance was strong for predicting fatigue presence, recall for the minority class (fatigue absence) remained low due to class imbalance.
