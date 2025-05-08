# COMS4761FinalProject

Load data with this code (as seen in first code block):

#https://archive.ics.uci.edu/dataset/15/breast+cancer+wisconsin+original

from ucimlrepo import fetch_ucirepo 
  
# fetch dataset 
breast_cancer_wisconsin_original = fetch_ucirepo(id=15) 
  
# data (as pandas dataframes) 
X = breast_cancer_wisconsin_original.data.features 
y = breast_cancer_wisconsin_original.data.targets 

Packages required for code:

ucimlrepo
imblearn
numpy
pandas
scikit-learn
sklearn
matplotlib
seaborn
umap-learn

pip install for any package listed above compatible with Python 3.6 and higher

Python 3.6 and higher must be installed for this code to run

Parameters:
dimension_reduction input must be 'pca’, 'umap' where the first will apply PCA and the latter UMAP as the dimension reduction technique n_components will be 2
classifier input must be 'svm’, 'logistic_regression’, 'random_forest' where the first will use an SVM model, the second a logistic regression, and the last a random forest model as the classification model
features input must be list of column names for all feature variables considered 
target input must be list format of the single target variable considered
df input must be the full dataset of the featuristic dataset

def pipeline(dimension_reduction, classifier, features, target, dataset)
