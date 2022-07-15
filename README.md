# Heart-disease-prediction
- Dataset used for heart disease prediction is available in kaggle and contains information regarding features like age,sex,chol,restecg,thal etc. The analysis focuses on which features are important in heart disease prediction and aid us in predicting heart diseases accurately..
- Initially data is imported into panadas dataframe via Jupyter notebook, checked for any missing,duplicate values and observed the data distribution of the independant features using matplot lib package.
- A heatmap was plotted between the correlations of the features which gives us an insight regarding the independant features that are important in predicting the diagnosis. 
- Next, categorical variable like 'sex', 'cp', 'fbs', 'restecg', 'exang', 'slope', 'ca', 'thal' are converted into numeric with the help of one hot Encoder.One hot Encoder is the part of pandas framework in Python and used to convert categorical data, or text data, into numbers, which our predictive models can better understand.
- Continuous variables like 'age','trestbps','chol','thalach','oldpeak' are scaled using Standard Scaler function from scikit learn preprocessing package.
- Data is then split into Training and testing data sets and a K-Nearest Neighbors regression was fit on the training data set where the parameters of Logistic Regression model were selected through Grid Selection.(One of the Hyper parameter Tuning Method).
- Precision score of K-Nearest Neighbors model on test dataset came out to be 0.90.
- Similarly, a random forest model was fit on the dataset and the parameters of random forest model were selected by grid selection method.
- Precision score of random forest model on test dataset came out to be 0.83 which indicates the fact that K-Nearest Neighbors is a better model for this dataset.
