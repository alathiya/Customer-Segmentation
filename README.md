# Content: Unsupervised Learning


## Project: Creating Customer Segments


In this project, I have analyzed a dataset containing data on various customers' annual spending amounts (reported in monetary units) 
of diverse product categories for internal structure. One goal of this project is to best describe the variation in the different types 
of customers that a wholesale distributor interacts with. Doing so would equip the distributor with insight into how to best structure 
their delivery service to meet the needs of each customer.



## Install


This project requires **Python 2.7** and the following Python libraries installed:


- [NumPy](http://www.numpy.org/)

- [Pandas](http://pandas.pydata.org)

- [matplotlib](http://matplotlib.org/)

- [scikit-learn](http://scikit-learn.org/stable/)



You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)



## Data



The customer segments data is included as a selection of 440 data points collected on data found from clients of a wholesale distributor 
in Lisbon, Portugal. For the purposes of this project, the features 'Channel' and 'Region' will be excluded in the analysis — with focus 
instead on the six product categories recorded for customers.More information can be found on the 
[UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).



Note (m.u.) is shorthand for *monetary units*.

**Features**


1) `Fresh`: annual spending (m.u.) on fresh products (Continuous); 

2) `Milk`: annual spending (m.u.) on milk products (Continuous); 

3) `Grocery`: annual spending (m.u.) on grocery products (Continuous); 

4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);

5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);

6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous); 

7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)

8) `Region`: {Lisbon - 1, Oporto - 2, or Other - 3} (Nominal) 

##Implementation

I have used Gaussian Mixture Model clustering algorithm to identify the various customer segments hidden in the data. Goodness
of clustering can be quantified from each data point's silhouette coefficient.The silhouette coefficient for a data point measures 
how similar it is to its assigned cluster from -1 (dissimilar) to 1 (similar). Calculating the mean silhouette coefficient provides 
for a simple scoring method of a given clustering. 

After running clustering algorithm on data silhouette score is reported for different number of clusters. Best silhouette score is 
chosen from predicted number of clusters. Finally visualization is done for optimal number of clusters. 
Conclusion is done with investigation on ways to use clustered data. 
  