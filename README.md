# Graph Machine Learning Final Project

<div align="justify">
  
Graph Neural Networks (GNN), which have been developed as a powerful candidate for modeling graph-structured data, are one of the hottest topics in recent years. A molecule can be naturally represented as a graph In it, atoms (vertices) are connected by chemical bonds (edges).

In this project we attempted to use **Graph Neural Networks** for **Classification** and **Regression** on molecular data. We implemented 6 GNNs. In the last one, we used edge features too. 

## Initial Atom, Bond, and Molecule-level Features of Datasets

Three features are extracted and utilized for each molecule: atom, bond, and molecule-level features. All features are computed rapidly in silico using the open-source package RDKit.

The initial atom and bond features are listed in the tables below. All features in these two tables are one-hot encodings except for atomic mass, an actual number scaled to be on the same order of magnitude.

[![1.png](https://i.postimg.cc/gr9pRVf1/1.png)](https://postimg.cc/GTj6ny3j)

[![2.png](https://i.postimg.cc/Wz18nxPk/2.png)](https://postimg.cc/CB9bMP5h)


## Graph Classification

Graph classification is the problem of determining the category or label of a graph. If we have a dataset consisting of a large number of input graphs, the problem is to classify each of the graphs into the correct target category or label. 

We used the **BBBP** dataset for the classification task. BBBP (Blood–brain barrier penetration) dataset comes from a recent study on the modeling and prediction of barrier permeability. This dataset records whether a compound is permeable to the blood-brain barrier.

### Results
We used the ROC-AUC metric to compute the score.

[![image.png](https://i.postimg.cc/02SBWMM5/image.png)](https://postimg.cc/RNMdq0L2)

# Graph Regression

Regression of graphs is similar to their classification and the difference is in the loss function and the performance metric. 

We used the FreeSolv dataset for the regression task. FreeSolv is selected from the Free Solvation Database, which contains the hydration free energy of small
molecules in water from experiments and alchemical free energy calculations.

### Results
We used the RMSE metric to compute the score.

[![image2.png](https://i.postimg.cc/vTRQ5THN/image.png)](https://postimg.cc/tZ5QjX63)


