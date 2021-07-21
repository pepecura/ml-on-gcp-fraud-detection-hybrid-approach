
## <font color='green'> **Fraud Detection in Financial Transactions** </font> 
In this notebook, we will work on a simulated transactions data for fraud detection. We will start with the analysis of fraud and create new features, then run machine learning models with BigQuery ML and Vertex Tables and evaluate the performance. Finally we will run the ML model to score a test dataset and export the predictions to BigQuery to take actions.
The public data used in the exercise is downloaded from the Kaggle website:
https://www.kaggle.com/ealaxi/paysim1

### <font color='green'> **Steps we follow:** </font> 
1. Download data </br>
2. Load data </br>
3. Explore data </br>
4. Prepare data </br>
5. Build unsupervised model using k-means in BigQuery ML </br>
6. Build supervised model using in BigQuery ML using XGBoost and Regression </br>
7. Deploy model and get prediction scores
