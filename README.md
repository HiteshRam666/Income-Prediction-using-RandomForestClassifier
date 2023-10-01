# Income💲💵-Prediction-using-RandomForestClassifier

## About Dataset

An individual’s annual income results from various factors. Intuitively, it is influenced by the individual’s education level, age, gender, occupation, and etc.

This is a widely cited KNN dataset. I encountered it during my course, and I wish to share it here because it is a good starter example for data pre-processing and machine learning practices.

## Fields
The dataset contains 16 columns

Target filed: Income

-- The income is divide into two classes: <=50K and >50K
Number of attributes: 14

-- These are the demographics and other features to describe a person

We can explore the possibility in predicting income level based on the individual’s personal information.

# Algorithm Used

- **A random forest classifier**.

A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. The sub-sample size is controlled with the max_samples parameter if bootstrap=True (default), otherwise the whole dataset is used to build each tree.

![how-random-forest-classifier-work](https://github.com/HiteshRam666/Income-Prediction-using-RandomForestClassifier/assets/116026459/6efa20b1-ab5e-4584-b681-df370ad2f839)

## Grid Search CV

GridSearchCV is the process of performing hyperparameter tuning in order to determine the optimal values for a given model. As mentioned above, the performance of a model significantly depends on the value of hyperparameters. Note that there is no way to know in advance the best values for hyperparameters so ideally, we need to try all possible values to know the optimal values. Doing this manually could take a considerable amount of time and resources and thus we use GridSearchCV to automate the tuning of hyperparameters.

GridSearchCV is a function that comes in Scikit-learn’s(or SK-learn) model_selection package.So an important point here to note is that we need to have the Scikit learn library installed on the computer. This function helps to loop through predefined hyperparameters and fit your estimator (model) on your training set. So, in the end, we can select the best parameters from the listed hyperparameters.

![81Yoo](https://github.com/HiteshRam666/Income-Prediction-using-RandomForestClassifier/assets/116026459/bfe13827-5704-4f49-a6a0-2eed5f7dd17b)
