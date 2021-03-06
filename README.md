# Machine Learning Notebooks
I collect various Jupyter notebooks of ML projects I worked on in this repository.

### Case Study 01 -- Mines vs Rocks (Binary Classification, Small Sample Issues)
This is a very small data set (208 rows) which is also wide (60 predictor variables). I investigated the effects of small sample size in the notebook. 
I tend to use the year we are in (2019 in this case) as the random number generator seed and I realized that I got very lucky in this dataset as a result; 
I got perfect recall! If I had worked on it in a different year, the result would have been drastically different. Therefore, I averaged the performance of 
my models using different seeds in order to reduce the variance.

### Case Study 02a -- Forest Cover Type (Multi-class Classification)
This is a dataset containing half a million instances on 54 predictor variables. The objective is to predict forest cover type (there are 7 different 
classes) from cartographic variables.

### Case Study 02b -- Forest Cover Type (Feature Importances and Selection)
We use the Forest Cover Type dataset to investigate feature importances and reduce the number of features without impacting accuracy thereby.

### Case Study 03a -- Wine Quality (Regression)
The dataset consists of physical and chemical properties of 6497 wines (1599 red and 4898 white) along with quality scores given to each instance by a panel of wine 
testers (median of at least 3 evaluations). Each expert graded the wine quality between 0 (very bad) and 10 (very excellent). The objective is to predict the quality 
score assigned to each wine by a group of experts using chemical properties as predictor variables.

### Case Study 04a -- Credit Card Fraud Detection (Binary Classification, Imbalanced Classes)
The datasets contains transactions made by credit cards in September 2013 by european cardholders. This dataset presents transactions that occurred in two days, where 
we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions. The objective is to 
identify fraudulent credit card transactions. We use asymmetric weights in the loss function (misclassification of the minority class is penalized more than misclassification 
of the majority class) to deal with the class imbalance in this notebook.

### Case Study 04b -- Credit Card Fraud Detection (Binary Classification, Imbalanced Classes, Over/Undersampling)
This is a continuation of the study of the  credit card fraud detection dataset. We use various over/undersampling methods (found in imbalanced-learn library) to deal with 
the class imbalance problem in this notebook.

### Case Study 04c -- Credit Card Fraud Detection (Binary Classification, Imbalanced Classes, Balanced Ensemble Methods)
This is the third notebook dedicated to the study of the credit card fraud detection dataset. This time we use ensemble methods found in imbalanced-learn library to 
deal with the class imbalance problem.


### Dimension Reduction 1 -- Fashion-MNIST
Fashion-MNIST is a dataset which contains 70000 everyday clothing items/accesories represented as a grayscale 28x28 image; hence, each instance lives in a 784 dimensional
space. We use various dimension reduction algorithms such as PCA, NMF, t-SNE, UMAP, and Isomap in order to reduce the dimension to 2 and visualize the dataset as a scatterplot 
thereby.

### Dimension Reduction 2 -- MNIST
MNIST is a dataset comprising 70000 hand-written digits represented as a grayscale 28x28 image; hence, each instance lives in a 784 dimensional
space. We use various dimension reduction algorithms such as PCA, NMF, t-SNE, UMAP, and Isomap in order to reduce the dimension to 2 and visualize the dataset as a scatterplot 
thereby.

### Dimension Reduction 3 -- Breast Cancer Dataset
The Breast Cancer (diagnostic) dataset contains 569 instances (212 malignant and 357 benign) with 30 numeric features which are computed from a digitized image of a fine 
needle aspirate (FNA) of a breast mass.  They describe characteristics of the cell nuclei present in the image. We use various dimension reduction algorithms such as PCA, 
NMF, t-SNE, UMAP, and Isomap in order to reduce the dimension to 2 and visualize the dataset as a scatterplot thereby.

### Support Vector Identification
When I was learning the theory of Support Vector Machines (SVM) from the awesome book titled 'An Introduction to Statistical Learning with Applications in R' of 
James, Witten, Hastie and Tibshirani (which is made freely available by the authors, hint: just google it), I had to disagree with the authors on a simple case of 
counting. In one of the figures (the bottom right one on page 348), the authors say that there are eight support vectors and I counted nine! (I am including the 
figure here for quick reference). As a result, I simulated some data, fitted SVMs, and identified the support vectors to check my understanding of the concept.
