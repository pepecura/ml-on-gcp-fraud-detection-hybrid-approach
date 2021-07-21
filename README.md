
## **Fraud Detection in Financial Transactions** 
In this notebook, we will work on a simulated transactions data for fraud detection. We will start with the analysis of fraud and create new features, then run machine learning models with BigQuery ML and Vertex Tables and evaluate the performance. Finally we will run the ML model to score a test dataset and export the predictions to BigQuery to take actions.
The public data used in the exercise is downloaded from the Kaggle website:
https://www.kaggle.com/ealaxi/paysim1

### **Steps we follow:** 
1. Download data </br>
2. Load data </br>
3. Explore data </br>
4. Prepare data </br>
5. Build an unsupervised model using k-means in BigQuery ML with **anomaly detection** feature </br>
6. Build supervised models in BigQuery ML and Vertex Tables </br>
7. Batch prediction </br>
8. Combining supervised and unsupervised model results for a **hybrid approach** to take action</br>

### **K-means model in BigQuery ML**
![image](https://user-images.githubusercontent.com/10263373/126524932-97a40361-1830-45c0-9eb6-9f112d4fc90e.png)
### **Vertex Tables model for Fraud Detection**
![image](https://user-images.githubusercontent.com/10263373/126524965-5d5a0f5b-7a09-4892-82b8-6f90366b66dc.png)
![image](https://user-images.githubusercontent.com/10263373/126525015-9a6d2d08-7529-4ad1-b8cf-a0b6e1b69998.png)

**Conclusion: The high scores from supervised model are selected for fraud investigation (95% of the selected group are fraudulent and this group includes 90% of the overall fraudulent transactions). In the final step, we analyse the observations that have slightly lower scores but show abnormal behaviour in the unsupervised model. Majority of those transactions are also seen as fraudulent so the number of false negatives are decreased with this hybrid approach.**
