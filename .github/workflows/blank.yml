def value_counts_df(df_column, count='count', drop_0=True):
    '''    
    * df_column - dataframe column 
    * count='count' - name of new number column containing value counts
    * drop_0=True - usefull if using this function on category type column, then there is posibility
    to recieve items with '0' count as a result
    '''
    column_name = df_column.name
    new_table = pd.DataFrame(df_column.value_counts())
    new_table.reset_index(level=0, inplace=True)
    new_table.columns = [column_name, count]
    if drop_0 == True:
        new_table = new_table[new_table[count]!=0]
    return new_table
