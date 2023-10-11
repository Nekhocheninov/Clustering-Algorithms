# Python DBSCAN

[DBSCAN](https://en.wikipedia.org/wiki/DBSCAN) clustering algorithm implementation in Python.

### Running the notebook

The code was written in Python across Jupyter notebooks. It was developed in Google Colab which is a free Jupyter notebook environment that allows you to run code through a browser.

Follow [this link](https://drive.google.com/file/d/1E2iCzuglv7Kz77-hEx0eq_tHeP3iZZNK/view?usp=sharing) to open the notepad with this code and click on Google Colaboratory.

# Samples

### Dataset

The datasets were taken from the scikit-learn.

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/DBSCAN/img/img_1.PNG" width="800">

### Analysis

Clustering of the first data set with the parameters of the minimum density of objects and the radius of the object’s surroundings, respectively: (3, 0.1), (3, 0.05), (5, 0.08), (7, 0.08).

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/DBSCAN/img/img_2.PNG" width="800">

Clustering of the second data set with the parameters of the minimum density of objects and the radius of the object’s surroundings, respectively: (3, 0.05), (3, 0.1), (2, 0.07), (10, 0.1).

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/DBSCAN/img/img_3.PNG" width="800">

Clustering of the third data set with the parameters of the minimum density of objects and the radius of the object’s surroundings, respectively: (3, 0.5), (5, 0.5), (5, 1), (16, 0.7).

<img src="https://github.com/Nekhocheninov/ClusteringAlgorithms/blob/main/DBSCAN/img/img_4.PNG" width="800">

All tests of the algorithm on the presented data sets are capable of unambiguous clustering with correctly selected parameters.

Let's compile a table of clustering accuracy for the third data set with the parameters of the minimum density of objects and the radius of the object's surroundings 16 and 0.7.
| | |
|---|---|
|Number of records in the sample | 500 |
|Number of correctly clustered objects | 472 |
|Number of incorrectly clustered objects | 0 |

### Conclusion

The DBSCAN algorithm is very simple and does not require specifying the number of clusters to search. It can deal with noise by removing it from the separation process. Clusters do not have to be linearly separable. However, it cannot manage clusters of different densities.
