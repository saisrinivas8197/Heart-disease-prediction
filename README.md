# Heart-disease-prediction
- Dataset used for heart disease prediction is available in kaggle and contains information regarding features like age,cholestrol levels,. The analysis focuses on which features are important in cancer prediction and aid us in model selection and hyper parameter selection.
- Initially data is imported into panadas dataframe via Jupyter notebook, checked for any missing or null values and observed the data distribution of the independant features using matplot lib package.
- Next, categorical variable (diagnosis) is converted into numeric with the help of Label Encoder.Label Encoder is the part of SciKit Learn library in Python and used to convert categorical data, or text data, into numbers, which our predictive models can better understand.
- A heatmap was plotted between the correlations of the features which gives us an insight regarding the independant features that are important in predicting the diagnosis. For better understanding, a Extra Trees Regressor was fit on top of the data and with the help of Extra Trees Regressor.feature_importance_ sector important fetaures were identified and considered for further analysis.
- Data is split into Training and testing data sets and a logistic regression was fit on the training data set where the parameters of Logistic Regression model were selected through Grid Selection.(One of the Hyper parameter Tuning Method).
- Precision score of Logistic model on test dataset came out to be 0.9556.
- Similarly, a random forest model was fit on the dataset and the parameters of random forest model were selected by grid selection method.
- Precision score of random forest model on test dataset came out to be 0.8 which indicates the fact that Logistic Regression is a better model for this dataset.
