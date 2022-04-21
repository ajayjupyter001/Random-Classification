# RANDOM CLASSIFICATION
## AIM:
To write a python program to perform random classification.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Google Colab /Jupiter Notebook

## Related Theoritical Concept:
NUMPY
NumPy is a library for the Python programming language, adding support for large, multidimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays.

SK LEARN
Scikit-learn is a free software machine learning library for the Python programming language. It features various classification, regression and clustering algorithms including support-vector machines.

MATPLOTLIB
Matplotlib is a plotting library for the Python programming language and its numerical mathematics extension NumPy. It provides an object-oriented API for embedding plots into applications using generalpurpose GUI toolkits like Tkinter, wxPython, Qt, or GTK.


## Algorithm
1.  Start the program.
2.	Import libraries required as per requirement.
3.	Define dataset use the make_blobs() function to generate a synthetic multi -class classification dataset.
4.	summarize dataset shape
5.	summarize observations by class label
6.	summarize first few examples
7.	plot the dataset and color the by class label
8.	stop the program


## Program:
```
/*
Program to implement random classification.
Developed by   : Ajay A
RegisterNumber :  212219040006
*/
```
```python
import matplotlib.pyplot as plt
from sklearn import datasets
X,y = datasets.make_blobs(n_samples=100,n_features=2,centers=2,cluster_std=1.05,random_state=2)

fig=plt.figure(figsize=(10,8))
plt.plot(X[:,0][y==0], X[:,1][y==0],'rs')
plt.plot(X[:,0][y==1], X[:,1][y==1],'go')
plt.xlabel("Feature 1")
plt.ylabel("Feaure 2")
plt.title("Random Classification Data with 2 classes")
```
## Output:
![image](https://user-images.githubusercontent.com/102233600/164498332-f16241c8-ff44-4448-a96e-0c049f4a3b36.png)




## Result:
Thus the random classifier was successfully implemented using python programming.
