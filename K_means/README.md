# Python k-means

[![Open in Colab](https://img.shields.io/badge/Open%20in%20Colab-Open-blue?logo=google-colab)](https://drive.google.com/file/d/1v8tzI5zChFRS1BJqkYvSlWKyGXfOwTB3/view?usp=sharing)

[K-mean](http://en.wikipedia.org/wiki/K-means_clustering) clustering algorithm implementation in Python.

## Running the notebook

The code was written in Python across Jupyter notebooks. It was developed in Google Colab which is a free Jupyter notebook environment that allows you to run code through a browser.

Follow [this link](https://drive.google.com/file/d/1v8tzI5zChFRS1BJqkYvSlWKyGXfOwTB3/view?usp=sharing) to open the notepad with this code and click on Google Colaboratory.

## Samples

### Dataset

The training and testing datasets were taken from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/), using the [Iris Dataset](https://archive.ics.uci.edu/dataset/53/iris).

The data set contains 3 classes of 50 instances each, where each class refers to a type of iris plant.  One class is linearly separable from the other 2; the latter are not linearly separable from each other.

### Analysis

We have histograms for each training set attribute value:

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/K_means/img/img_1.PNG" width="800">

We can also compare the attributes of the training dataset:

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/K_means/img/img_2.PNG" width="800">

Based on the previous image, we can observe a clearly separable class.

Iris-setosa is linearly separable from the other two classes; Iris-versicolor and Iris-virginica are not linearly separable (blue - Iris-setosa, red - Iris-versicolor, green - Iris-virginica):

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/K_means/img/img_3.PNG" width="800">

Let's find cluster centers using our code:

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/K_means/img/img_4.PNG" width="800">

Comparison of sepal_width and sepal_length attributes does not make it possible to uniquely determine the cluster centers, as shown in the previous figure.

Accuracy table for 5 test algorithm:

| № |	sepal_width-sepal_length |	petal_width-petal_length |
|---|---|---|
|1 |	***0.53(3)*** |	0,96(6) |
|2 |	0.3(3) |	0.95 |
|3 |	0.3(3) |	***0.983(3)*** |
|4 |	0.3083(3) |	0.475 |
|5 |	0.0416(6) |	0.63(3) |

The best clustering result was obtained when comparing the petal_width-petal_length attributes.

### Conclusion

The k-means algorithm is iterative. The number of iterations of the algorithm is generally not fixed and depends on the initial location of objects in space; the number of clusters k is an input parameter; as well as on the initial approximation of the centers of clusters. Also, if the initial parameters are not selected successfully, the iterative process can converge to the local optimum. For these reasons, the algorithm is not deterministic and robust.
