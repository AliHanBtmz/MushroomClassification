<h1 align='center'> Mushroom Classification</h1>
<h2> Project purpose:</h2>
<p>Project Purpose: To create a model that allows the binary classification of mushrooms as edible and poisonous.</p>

## About Dataset
This dataset is a cleaned version of the original Mushroom Dataset for Binary Classification Available at UCI Library. This dataset was cleaned using various techniques such as Modal imputation, one-hot encoding, z-score normalization, and feature selection. It contains 9 columns:

* Cap Diameter
* Cap Shape
* Gill Attachment
* Gill Color
* Stem Height
* Stem Width
* Stem Color
* Season
* Target Class - Is it edible or not?
  <p></p>
The Target Class contains two values - 0 or 1 - where 0 refers to edible and 1 refers to poisonous.

## Model training and The Most Efficient Algorithm
 
<b>Accuracy scores:</b>
* Logistic Regression => 0.636531877486814
* Decision Tree => 0.978532432682520
* K-Nearest Neighbor => 0.990099009900990

<p>Model training with 3 different algorithms. K-Nearest Neighbor algorithm gave the highest accuracy among them. If we were to explain this algorithm:</p>

<h3>KNN Model</h3>
This report is prepared to explain the basic principles of the K-Nearest Neighbors (KNN) algorithm and to describe how it is used within the context of a sample project. KNN is fundamentally a classification or regression algorithm that classifies or predicts data points based on their nearest neighbors. This report elaborates on how KNN works, how the model is built and used, and also illustrates how KNN is applied in a sample project context.

<h3> Working Principle of KNN</h3>
The KNN algorithm finds the K nearest neighbors to classify or predict a data point, utilizing the classes or values of these neighbors. At its core lies the concept of similarity or distance. Euclidean distance is often used as a distance metric to measure the distance between data points. The main parameters of KNN include K (number of neighbors) and weights (weights of neighbors). While the K parameter determines the number of nearest neighbors, the weights parameter defines the influence of neighbors on classification or prediction.

<h3>Model Construction</h3>
When constructing the KNN model, firstly an object is created from the KNeighborsClassifier class. This object is initialized with parameters such as n_neighbors and weights. For instance, the parameter n_neighbors=10 indicates that the model will use 10 neighbors, while the parameter weights='uniform' specifies that all neighbors have equal weight.

<p></p>

<p>KNNClassifierModel = KNeighborsClassifier(n_neighbors=10, weights='uniform',algorithm='auto')</p>

<h3>Model Utilization</h3>

The constructed KNN model is trained on the dataset and then used to make predictions for new data points. The fit() method is used for training.

<h3>Evaluation of Model Performance</h3>
The model performance is evaluated using predetermined metrics. Accuracy is commonly used as a metric, along with the representation of a confusion matrix.
