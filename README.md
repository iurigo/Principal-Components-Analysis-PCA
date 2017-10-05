# Principal-Components-Analysis-PCA
![](https://github.com/iurigo/Principal-Components-Analysis-PCA/blob/master/assets/images/pca_coordinate_transformation.png)

PCA is a very popular technique for performing "dimensionality reduction" on your data.
Dimensionality reduction is the process of combining or collapsing your existing features (columns in X) into new features that not only retain the original information (or as much of it as we can) but also ideally reduce noise.

#### Reminder:
PCA is a pre-processing step. It is not a model.

#### What is PCA?
PCA finds the linear combinations of your current predictor variables that will create new "principal components" that explain, in order, the maximum possible amount of variance in your predictors.

Intuitively, PCA transforms the coordinate system so that the axes become the most concise, informative descriptors of our data as a whole.
The new axes are the principal components.

#### The Process of PCA
Say we have a matrix $X$ of predictor variables. PCA will give us the ability to transform our $X$ matrix into a new matrix $Z$.
We will derive a weighting matrix $W$, made up of the eigenvectors of the covariance matrix of $X$, that allows us to perform the transformation.
Each successive dimension (column) in $Z$ will be rank-ordered according to variance in its values!

#### There are 3 assumptions that PCA makes:
1. Linearity: Our data does not hold nonlinear relationships.
2. Large variances define importance: our dimensions are constructed to maximize remaining variance.
3. Principal components are orthogonal: each component (columns of $Z$) is completely un-correlated with the others.
