Goal- 
The dataset contains poems and their genre. Their are 4 genres in the dataset- Music, Death, Environment, Affection. Make a multiclass classification model, which will predict the genre of the poem by analyzing the poem.


Solution Approach- 
I have cleaned the data then did data preprocessing which included- removing stopwords, stemming, TF-IDF to convert text into numerical features.
Then I created 10 models using 5 classifiaction algorithms. 
Classification algorithms used are Multinomial Naive Bayes, Random forest, SVM, LogisticRegression and XGBoost.
For each  classification algorithm, I have made 2 models- 1 using hyperparameter tuning (using RandomizedSearchCV) and another using default values of parameter for algorithm.
Each model is evaluted using classification matrix and accuracy.


Detailed steps for making the models-
Import the required libraries and load the dataset.
Remove rows which have null values and remove duplicate rows.
Shuffle the dataset.
Check the number of poems in each genre.
Music              238
Death              229
Environment        227
Affection          141
Since there is not much variation in the number of observations in all classes so we don't need to do oversampling or undersampling.
Remove stopwords.

Do stemming.

Convert Poem column(text) into numerical features using TF-IDF.

Divide dataset into train and test set.

I have created 10 models using 5 classifiaction algorithms. 

Classification algorithms used are Multinomial Naive Bayes, Random forest, SVM, LogisticRegression and XGBoost.
For each  classification algorithm, I have made 2 models- 1 using hyperparameter tuning (using RandomizedSearchCV) and another using default values of parameter.

This way, 10 models are made-
1. Hyperparameter tuned Multinomial Naive Bayes-
2. Default Multinomial Naive Bayes
3. Hyperparameter tuned random forest
4. Default Random Forest
5. Hyperparameter tuned SVM
6. Default SVM
7. Hyperparameter tuned LogisticRegression
8. Default Logistic Regression
9. Hyperparameter tuned XGBooost
10.Default XGBoost
Each model is evaluted using classification matrix and accuracy.
