# value_counts_df
modified pandas value_counts() function that makes a new value_counts dataframe as a result

* df_column - dataframe column 
* count='count' - name of new number column containing value counts
* drop_0=True - usefull if using this function on category type column, then there is posibility to recieve items with '0' count as a result
