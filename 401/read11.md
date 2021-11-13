# JupyterLab
is a next-generation web-based user interface for Project Jupyter.

JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner

JupyterLab understands many file formats (images, CSV, JSON, Markdown, PDF, Vega, Vega-Lite, etc.) 

--------------------------------------------


# NumPy ( Data Analysis with Python )
By using NumPy, you can speed up your workflow

**how to extract data from csv file and convert it to list of lists:**

        import csv
        with open('winequality-red.csv', 'r') as f:
            wines = list(csv.reader(f, delimiter=';'))

**how to make a matrix using NumPy**

        import csv
        with open("winequality-red.csv", 'r') as f:
            wines = list(csv.reader(f, delimiter=";"))
        import numpy as np
        wines = np.array(wines[1:], dtype=np.float)


**to display how many rows and column inside 2D-array:**

        wines.shape


**to create an array with # of rows and columns with zeros**

        empty_array = np.zeros((3,4))

**to create an array with # of rows and columns with a random numbers**

        np.random.rand(3,4)


**you can use NumPy to open csv files**

        wines = np.genfromtxt("winequality-red.csv", delimiter=";", skip_header=1)
        # skip_header: to skip header row 


**to find the data type of the NumPy arrays**

        wines.dtype


**to convert the data type of the NumPy arrays**

        wines.astype(int)

## Broadcasting
broadcasting involves a few steps:

- The last dimension of each array is compared.
    - If the dimension lengths are equal, or one of the dimensions is of length 1, then we keep going.
    - If the dimension lengths aren’t equal, and none of the dimensions have length 1, then there’s an error.
- Continue checking dimensions until the shortest array is out of dimensions.


***resources**
 [ numpy](https://www.dataquest.io/blog/numpy-tutorial-python/#)