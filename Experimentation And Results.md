### EXPERIMENTATIONS AND RESULTS 🧪📊

**Detailed Explanation:**
The "Experimentations and Results" section provides an in-depth analysis of the methods and outcomes of testing various machine learning models to predict the remaining useful life (RUL) of lithium-ion batteries. This section involves the following key steps:

1. **Dataset Analysis**:
    - The dataset comprises 124 commercial lithium-ion phosphate (LFP) and graphite cells (APR18650M1A) cycled to failure under controlled conditions. These cells have a nominal capacity of 1.1 Ah and a nominal voltage of 3.3 V.
    - Data includes measurements of charge capacity, discharge capacity, internal resistance, temperature, current, and voltage over approximately 760 life cycles.
    - Charging policies varied, with some cells undergoing one-step or two-step charging. Charging times ranged from 8 to 13.3 minutes, capturing a wide range of cycle lives (150 to 2300 cycles).

2. **Data Preprocessing**:
    - **Normalization**: Standardization of datasets was performed to eliminate the negative effects caused by different ranges of values, reducing data redundancy and improving data integrity. This process involves scaling the features to have a mean of zero and a standard deviation of one.
    - **Splitting the Data**: The dataset was divided into training and testing sets in a 75:25 ratio to evaluate the performance of the models accurately. 

3. **Model Training and Evaluation**:
    - Six machine learning models were employed: Deep Neural Network (DNN), Gradient Boosting Trees (GBT), Naïve Bayes, Principal Component Analysis (PCA), Linear Discriminant Analysis (LDA), and Kernel PCA.
    - The models were trained on the training set and evaluated on the testing set to compare their performance in predicting the battery life.
    - **Deep Neural Network (DNN)**: Utilized three hidden layers and one output layer. The "relu" activation function was used in the hidden layers, and the "softmax" function in the output layer. The model was optimized using the "adam" optimizer, with a batch size of 10 and 100 epochs.
    - **Gradient Boosting Trees (GBT)**: Comprised an ensemble of weak prediction models (decision trees) built in a stage-wise manner. The model was set with a maximum depth of 2, 20 estimators, and a learning rate of 0.1.
    - **Naïve Bayes**: Applied Bayesian theorem with the assumption of conditional independence between features. This model was implemented using the GaussianNB classifier from the sklearn library.
    - **Principal Component Analysis (PCA)**: Reduced dimensionality by transforming correlated variables into uncorrelated principal components. The model used two principal components followed by a Logistic Regression model.
    - **Linear Discriminant Analysis (LDA)**: Reduced dimensionality by projecting features into a lower-dimensional space, focusing on maximizing the separation between different classes.
    - **Kernel PCA**: Extended PCA by using kernel methods to project data into a higher-dimensional feature space, making it linearly separable. The model used two components with a radial basis function (rbf) kernel.

4. **Results and Interpretation**:
    - The performance of each model was evaluated based on accuracy. The results were summarized in a bar graph (Fig. 3) and an accuracy table (Table 2).
    - **Deep Neural Network (DNN)**: Achieved the highest accuracy of 89.44% on the testing set, demonstrating its effectiveness in predicting battery life.
    - **Principal Component Analysis (PCA)**: Showed strong performance with an accuracy of 87.23%, making it the second-best model.
    - **Kernel PCA**: Ranked third with an accuracy of 84.86%.
    - **Naïve Bayes**: Achieved an accuracy of 83.29%, indicating its robustness despite its simplicity.
    - **Gradient Boosting Trees (GBT)**: Demonstrated an accuracy of 80.88%, showing it as a competitive model.
    - **Linear Discriminant Analysis (LDA)**: Had the lowest accuracy of 79.37%, highlighting areas for improvement.
    - The models were prevented from overfitting, ensuring better generalization to new data.

5. **Correlation Analysis**:
    - Pearson’s coefficient of correlation was used to determine the relationship between the features and the cycle number.
    - **Voltage**: High correlation (0.984) with cycle number, indicating its significance in predicting battery life.
    - **Current**: Low correlation (0.174), suggesting it is less impactful.
    - **Charge Capacity**: Strong correlation (0.891), making it a key predictor.
    - **Discharge Capacity**: High correlation (0.922), emphasizing its importance.
    - **Internal Resistance**: Very high correlation (0.992), marking it as a critical factor.
    - **Temperature**: Negative correlation (-0.221), indicating a different type of influence on battery life.

**Layman Explanation:**
This part of the study details how they tested various computer models to predict how long batteries would last. They used data from 124 batteries, measuring important factors like how much charge the batteries could hold, their internal resistance, temperature, current, and voltage over about 760 uses.

1. **Analyzing the Data**:
    - They collected detailed information from each battery and tested them under different conditions to get a wide range of results.
2. **Preparing the Data**:
    - They standardized the data, meaning they adjusted it so that all the different factors were on the same scale, which helps the computer models work better.
    - They divided the data into two parts: one for training the models and one for testing them.
3. **Training and Testing the Models**:
    - They trained six different computer models using the training data and then tested how well each model could predict battery life using the testing data.
    - The Deep Neural Network (DNN) model was the best at predicting battery life, with an accuracy of about 89%.
    - The PCA model also performed well, with an accuracy of about 87%.
    - They made a bar graph to show the accuracy of each model.
4. **What They Found**:
    - The models were able to make accurate predictions without overfitting, which means they can generalize well to new data.
    - They identified which factors (like voltage, charge capacity, and internal resistance) were most important in predicting battery life.

**Importance:**
1. **Comparative Analysis**: Evaluating different models helps identify the most effective approach for predicting battery life.
2. **Data Standardization**: Ensuring all data is on the same scale is crucial for improving model performance.
3. **Practical Applications**: Accurate predictions can lead to better battery management, safety, and cost savings.

**Context Related to Overall Goal:**
The experiments and results section is critical for validating the effectiveness of the proposed machine learning models. By systematically testing and comparing different models, the study aims to find the most accurate method for predicting the remaining useful life of lithium-ion batteries, which is the primary goal of the research.

**Math Intuition and ML Terminologies:**
- **Standardization**: Transforming data to have a mean of zero and a standard deviation of one.
- **Training Set**: The portion of the data used to train the models.
- **Testing Set**: The portion of the data used to evaluate the model's performance.
- **Accuracy**: A measure of how close the predictions made by the model are to the actual outcomes.
- **Overfitting**: When a model learns the training data too well, including noise and details, leading to poor performance on new data.
- **Pearson’s Coefficient of Correlation**: A measure of the linear correlation between two variables, ranging from -1 to 1.

The experiments and results section highlights the rigorous process of testing and validating the proposed models, ensuring that the predictions made are reliable and accurate. This section provides a comprehensive analysis of the data and the performance of various models, contributing to the overall goal of accurately predicting battery life. 📊🔋🤖

## **Table of Contents:**
---
1. [Abstract](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/edit/main/README.md)
   
2. [Introduction](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/blob/main/Introduction.md) 

4. [Dataset Deatils](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/blob/main/Dataset%20Deatils.md) 

5. [Machine Learning Approaches And Models](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/blob/main/Machine%20Learning%20Approaches%20And%20Models.md) 

6. [Proposed Model](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/blob/main/Proposed%20Model.md)

7. [Experimentation And Results](https://github.com/aditya-saxena-7/Lithium-Ion-Battery-Life-Prediction-Based-on-Initial-Stage-Cycles-Using-Machine-Learning/blob/main/Experimentation%20And%20Results.md)
