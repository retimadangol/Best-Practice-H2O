
### Setting up H2O clusters:


There is no official documentation per say as to set sparkling water environment and resources for it can vary dramatically depending on the need.

However, these are just the guidelines:

The formula for "Total Memory" estimation from the link below should help:

(http://docs.h2o.ai/h2o/latest-stable/h2o-docs/faq/hadoop.html#what-amount-of-resources-are-used-and-reported-back-to-yarn) 
 
(http://docs.h2o.ai/h2o/latest-stable/h2o-docs/welcome.html#limiting-cpu-usage)


#### And these rules and the formula should help to work out the settings as well:

Set the correct cluster size for your given dataset size. The rule of thumb is to use at least 4-5 times the size of your data. 

##### For example:

if the dataset is 10GB, you should allocate at least 40GB of memory.
make sure that driver and executor memory are the same, 4gb or more and make sure driver and executor cores are 2 or more.
Try to limit the number of nodes to 8 or less

### If you are using Xgboost:

you would need to split the memory into 1/2 between xgboost and native, also taking into account that memory should be about 4 times the dataset size you will be using.

vcores will not affect h2o, and should use following references:
   
