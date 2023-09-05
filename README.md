# Project 4
Are you a good credit card client?? 

Group members: Jessica Clewis, Nikita Jain, Stephen Roberts, Khayria Ibrahim higo

Dataset: https://www.kaggle.com/datasets/rikdifos/credit-card-approval-prediction

Our dataset includes socio-economic and credit card payment status information for over 400,000 clients. talk about tableau visuals 

Our objective for this project is to build a machine learning model to predict if a client is “good” or “bad” based on the information given in the data set. We retrieved data using SQLite and used Pandas to read and merge the CSV files. 

Would a Logistic regression model be best to use? We started by cleaning the data by dropping unnecessary columns, renaming columns, and adding columns to assign 0 for “good” clients or 1 for “bad” clients. Using a standard scaler to train the score, we could create the Logistic regression classification model. The initial accuracy was 49% and after changing to inner join, the accuracy increased to 50%  the result in recall values was 0%. We thought we might be able to get a higher accuracy result, so we used the data to resample to get higher accuracy after we tested the accuracy increased to 52%. we used  Random Forest a  machine-learning model to test the data set, and the accuracy increased  by 67% 

What about unsupervised learning? We used similar methods as mentioned before to start with cleaned data. We used K-means and birch to cluster applicants based on (STEPHEN TO INSERT COLUMNS). We used the cluster values as labels for a logistic regression model to receive an accuracy score of 99%. Wait…is that right? Seems too high….

Would deep learning give results that are just right? We did not drop any columns this time before using the data. We optimized the neural network model by using various activation sets including Sigmoid, reLU, and Tanh. After generating classification reports and evaluating the model, we ended up with an accuracy score of 86%. 

When first looking at our data set, we realized there were only two outcomes: good or bad. This could explain the extremely high accuracy of the unsupervised learning model. Also, we began with 90% of the data representing good clients and bad making up only 10% of the data. The model doesn't want to learn about bad clients due to no fault of its own. There just isn’t much data represented by bad clients. This data imbalance most likely explains the 86% accuracy of the deep learning model being closely related to the 90% of our data being classified as "good" clients. 

