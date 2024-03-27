# Multi-Class-Cyber-Attack-Detection-Using-Ensemble-Learning

This project basically predicts 4 types of Attacks - DDos, U2R, R2L and Probe with the help of Ensemble Learning model.
First we create the dataset using Penetration Testing in Virtual Machines. The Virtual Machines we used for penetration testing are **KAli Linux** and **metasploitable**.
We  obtained the dataset from **wireshark** , saved the pcap file , converted the pcap into csv using a Python script.

Then we applied data preprocessing to remove the null values and visualize the dataset using matplotlib  data visualization techniques(pie chart, histogram ,etc).
We applied encoding techniques on the feature columns to convert into int64 data type. Then we split our dataset into 30% of the actual dataset for testing and the rest 67% for training.

After that we train 5 classification models - KNN, Decision Tree, Random Forest , Logistic Regression , Multinomial Naive Bayes and the accuracy found by each  of the models are 99.06%, 99.69%, 99.86%, 81.1%, 44.97% respectively.
Then we save the models in pickle files , load the models and perform the detection using Ensemble learning appraoch . 

We also analyze the accuracy of Bagging and Boosting approach in which boosting gives a fairly better accuracy and precision  compared to bagging.
