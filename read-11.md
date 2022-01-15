# Data Analysis

## Jupyter Lab

- JupyterLab is a next generation web-based user interface for Project Jupyter
- Code consoles provide scratchpads for running code
- Kernel backed documents enable code in any text file to be run interactively
- Notebook cell outputs can be mirrored into their own tab

## NumPy

- Numpy is a data analysis package
- In Numpy we will work with 2-D arrays or a matrix
- To create a Numpy Array we will use the `numpy.array` function and passing in a list of lists
- `tablename.shape` checks the number of rows and columns in our data
- To create an empty array use:`import numpy as np` 
  `empty_array = np.zeros((rows,columns))`
- To create an array with random numbers we us `np.random.rand(3,4)`
- To read a file use: `np.genfromtxt("filename",delimiter=";",skip_header=1)`
- Use indexes to pull data from Arrays [row,column]
- Slicing allows us to pull multiple items: `[0:3,3]` pulls first 3 items from the fourth column
- To assign values we can use index: `array[1,5]=10`
- To manipulate entire rows we can use slicing: `array[:,10]=50`
- To convert data types use: `array.astype(int)`
- Simple Array math is allowed as well. Using splicing to identify which items you would like to manipulate
- `numpy.ndarray.mean` finds the mean of an array.
- `numpy.ndarray.std` finds the standard deviation of an array.
- `numpy.ndarray.min` finds the minimum value in an array.
- `numpy.ndarray.max` finds the maximum value in an array.
- [Array Methods](https://numpy.org/doc/stable/reference/arrays.ndarray.html)

# Useful Links

- [NumPy Tutorial](https://www.dataquest.io/blog/numpy-tutorial-python/)
- [Jupyter](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html)