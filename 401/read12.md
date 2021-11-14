# pandas 
panda is a library in python for data analysis dealing with data in smooth way and easy

by using panda you can load, prepare and mainuplate moduls by join, manage, shap...etc data 

we can import panda
`import pandas as pd`

## panda usage
1. create object


        df2 = pd.DataFrame(
            {
                "A": 1.0,
                "B": pd.Timestamp("20130102"),
                "C": pd.Series(1, index=list(range(4)), dtype="float32"),
                "D": np.array([3] * 4, dtype="int32"),
                "E": pd.Categorical(["test", "train", "test", "train"]),
                "F": "foo",
            }
        )

2. Viewing data
    - to show head of data

            df.head()

    - to show the tail of data

            df.tail()

    - to show the index

            df.index

    - to show columns

            df.columns

    - shows a quick statistic summary of your data

            df.describe()

**`DataFrame.to_numpy()` gives a NumPy representation of the underlying data**


3. Selection by label

        df.loc[dates[0]]

4. Boolean indexing

        df[df["A"] > 0]

5. Missing data: pandas primarily uses the value np.nan to represent missing data


there is a lot of usage of panda for more

[10 minutes to pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)