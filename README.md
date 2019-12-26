# Classification-Model-Training-on-Titanic-Dataset
Data Pre-processing, EDA and training 8 different models and evaluation on Titanic Dataset

![alt text](https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png "Logo Title Text 1")

## Libraries used:
1. Numpy
2. Pandas
3. Matplotlib
4. Seaborn
5. Scikitlearn
6. Scikitplot

## Data
Dataset used in this notebook can be downloaded from: https://www.kaggle.com/c/titanic/data

## Steps done in this notebook:
1. Exploratory Data Analysis on the dataset
2. Checking variable distributions
3. Checking multi-variate correlations
4. Feature Engineering
5. Model Trainings

### 1. Exploratory Data Analysis
  In this step, inspecting the dataset(fields and meaning), inspecting missing values and outliers are done. No further handlings are done in this step. Missing values are handled in the feature engineering step(step 4). 
  
### 2. Checking variable distributions
  Distribution of a single variable is important as it can tell how the values are spread within the feature. Both numerical and categorical distribution inspections are done in this step using python's seaborn and matplotlib libraries.
  
### 3. Checking multi-variate correlations
  Other than the distribution of the variables, correlations can tell a lot about the data. It can tell the correlation between two or more variables and can also point out the dependency of the dependent(target) and independent(feature) variables within your dataset which can later impact on the model building step(step 5).
  
### 4. Feature Engineering
  The required feature transformations and handlings from step 1 like inspected missing values are handled in this step. Features with missing values are either removed completely or imputed in this step. Features with more than 70%(like Cabin) of missing values are removed and other features with missing values less than 20%(like Age, Embarked, Fare) are imputed with different methods(binning for Age, mode imputation for Embarked and mean imputation for Fare). Some features with big correlation like Sibling Number and Children Number are merged into Family Number feature. 
  
### 5. Model Trainings
   In this final step, the complete and cleaned data are finally dummified to be ready for model training. Different models like logistic regression, GaussianNB, BernoulliNB, KNN, SVC, Random Forests and boosting methods are tried and evaluated on this dataset. 
