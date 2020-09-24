
## How to get logs

Below are methods that could download logs for Python or R code.


### R:

```h2o.downloadAllLogs(filename = 'R_logs')```

### Python:

```h2o.download_all_logs('logs_in_Py')```

Or to increase the log file limit when launching Python: ```h2o.init(max_log_file_size="128MB")```

you can use ```max_log_file_size``` option to increase the log file limit

**It doesn't seem to be available if launching in R, at the moment, but looking to add it.


### Java cli:

It can be added to as: ```java -jar h2o.jar -max_log_file_size 128MB```



## Getting Logs from H2O flow

## On flow:

- On the top there is ```Admin``` button, 

- Click the drop down, you can see ```View log``` or ```Download logs``` button

- ```Download logs``` option will downloads the zip file 

- However, if downloading the log in zip is not an option click ```View log``` option and copy paste it on text file or word 
