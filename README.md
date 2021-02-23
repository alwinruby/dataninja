# Python Data Ninja

import numpy as np
import pandas as pd
from pandas import Series, DataFrame

print('Modules are imported.')



What is the basic syntax to create a Series?

    s = Series(data, index=index)


DataFrame accepts many different sorts of input...what is one of them?

    A Series


How would you go about making only certain columns appear in a DataFrame? Let's assume you have 3 columns, named column1, column2 and column3, and we want only column1 and column3

    DataFrame(nameOfYourDf, columns = ['column1', 'column3'])


How would we assign a value of 7 to column2 from the last question?

    nameOfYourDf['column2'] = 7


You have 5 columns and 5 rows, how would you make the last 4 rows appear?

    nameOfYourDf.tail(4)


Question 1: What would the following code result in:    df.dropna(axis=1, how='any')

            Any columns that has missing values would be dropped


Question 2: What would the following code result in:    df.dropna(thresh=4)

            Each row would have to have 4 data points to remain


Question 3: What would a right outer join accomplish when you're combining two dataframes?

            It would keep everything in the right dataframe


Question 4: Ordering your Columns can be helpful in presenting data more clearly, how would you accomplish such a goal?

            df = df[['Category', 'Sales', '# of Customers']]
