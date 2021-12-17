# Data Analytics

Description of Dataset

This dataset represents the activity of a large number of customers who are interested in buying policies from an insurance company. Each Quote_Id corresponds to a potential customer and the Quote_Flag indicates whether the customer purchased a policy or not. The provided features are anonymized and provide a rich representation of the prospective customer and policy. They include specific field, coverage, sales, personal, property and geographic information.

I had used Python to curb the problem classification of “Quote_Flag”, which is representing customer purchased the policy or not. Datset has 30 columns and I used all columns as features based on some criteria except “Quote_Id”, “Quote_Date” and “Quote_Flag”. Quote_Flag was that we have to predict on basics of X-features.

Input

A training dataset provide with the task I have to predict the labels of unknown data set. I used features for training based on various feature selection techniques. 

Output

Predicted quote flags with relevant quote ID on a excel file for submission on Kaggle.


Pre-Processing

All features in training data set were not directly use able for models. There were some categorical features and numerical features. In case of numerical features all important features were use able for the training except one It was having about 50% null values in it and its amputating with values was risk to model accuracy. So as feature was also not import upon results mention below from variable selection techniques. Categorical feature and textual features by clearing the null values among some features and conversation of textual data into numerical values based on unique text and category.  All columns’ data type was converting into numerical and null values problem was also curbed to step ahead towards solving problem.
Minmax scalar and Normalization  from learn is applied to numerical features.


Feature Selection

Below are some visuals about different techniques to show the important and multiple factors among all features with respect to label the of Quote Flags.
Extra Tree classifier uses a model to select the importance of features on certain factors by fitting and transforming the features with respect to label and by trying subsets of all features to predict the label. It is automated way to select the features but in some type of data it’s results not gave the perfect subset of features. Other than that, also used feature importance by the premutation among the variables before fitting to the model. Moreover, that for finding the importance of feature I had calculated the sequential forward that shows the importance of features in backward direction. Feature’s importance is also analysed by the mutual information score among all feature how they are mutually having information to predict the label. Finally, I had calculated the Persons cordiality coeffect of features with labels (negative value tells the inverse relation of variable with label, as negative value increases a negative effect on labels also increases, 0 empress no relation with label, Positive is vice versa of Negative).Chi Squad test is also allied to find the best features among the data.
