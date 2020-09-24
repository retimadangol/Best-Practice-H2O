
When converting the data from spark frame to h2o frame to pandas frame etc.
To have consistence data type declared in h2o, you want to import h2o frame with dtype declared as from previous frame data types:

#### Example for checking unique value of a column in spark frame and h2o frame:  

#get you dtype 

```data_types = {x:y for x, y in spark_df.dtypes}```

#pass same dtype in h2o dataframe

```h2o_df= h2o.import_file(data_path, col_types=data_types)```

#use group by:

```h2o_df.group_by(col_interested).get_frame().shape[0] == spark_df.select(col(col_interested)).distinct().count()```
