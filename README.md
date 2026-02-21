# Experiment – 8
## Title :
Tools For Exploratory Data Analysis - NumPy
## Aim :

To study and implement the NumPy library in Python and perform different numerical, multidimensional, and statistical operations for Exploratory Data Analysis.

## Objectives :

To understand what N-dimensional arrays (ndarrays) are

To learn how NumPy manages memory in numerical computing

To create arrays and check their properties

To perform mathematical and vectorized operations

To understand the difference between views and copies

To apply basic statistical and linear algebra operations for data analysis

### Theory on NumPy :

NumPy (Numerical Python) is one of the most important libraries used in Python for scientific and numerical computing. It provides support for large multi-dimensional arrays and matrices, along with many mathematical functions to operate on them.

The main object in NumPy is called an ndarray, which stores elements of the same data type.

### Architecture of ndarray :

Unlike normal Python lists, NumPy arrays are stored in a continuous block of memory. This means all elements are stored next to each other.

Because of this continuous storage, NumPy can access and process data much faster than Python lists.

### Characteristics of NumPy :
1. Vectorization :

Vectorization means performing operations on entire arrays without using loops.
This makes the code shorter and faster.

2. Homogeneity :

All elements in a NumPy array must be of the same data type.
This helps NumPy manage memory efficiently.

3. Striding :

Striding tells NumPy how many bytes it should move in memory to access the next element.

4. Broadcasting :

Broadcasting allows NumPy to perform operations on arrays of different shapes without manually resizing them.

5. Axis and Rank :

In NumPy, dimensions are called axes.
The number of axes is called the rank of the array.
For example:

A 1D array has 1 axis

A 2D array has 2 axes (rows and columns)

### Deep Dive into Core Operations :
#### 1. Memory Management – Views vs Copies :

When we slice a NumPy array, it creates a view instead of a copy.
This means the new array shares the same memory as the original array.

If we change the view, the original array also changes.

To create a completely separate copy, we use the .copy() method.

#### 2. Universal Functions (ufuncs) :

A ufunc is a function that works on each element of an array.

Some common examples are:

np.add

np.sin

np.exp

These functions are faster than using normal Python loops.

#### 3. Advanced Indexing :

NumPy supports:

Fancy Indexing

Using an array of indices to access multiple elements at once.

Boolean Indexing

Using True/False conditions to filter data.

Example:

data[data > 0]

This returns only the positive values from the array.

NumPy in the Data Science Ecosystem :

NumPy is widely used in data science and works together with other libraries:

Pandas – Built on NumPy; DataFrames use NumPy arrays internally.

Scikit-learn – Uses NumPy arrays for machine learning models.

Matplotlib – Uses NumPy arrays for plotting graphs.

SciPy – Extends NumPy with more advanced scientific functions.

### Applications of NumPy in EDA :

Dimensionality Reduction using techniques like PCA

Noise filtering using Fourier Transform

Data normalization and scaling

Generating random data for simulations

## Conclusion :

NumPy is a very important library for numerical computing in Python.
It makes calculations faster and more efficient compared to normal Python lists.

Because of its speed, memory efficiency, and ability to handle multidimensional data, NumPy is very useful for Exploratory Data Analysis and data science applications.
