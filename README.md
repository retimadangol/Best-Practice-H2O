# Best-Practice-H2O

## How to get logs

Below are methods that could download logs for Python or R code.

Python:

```h2o.download_all_logs('logs_in_Py')```

R:

```h2o.downloadAllLogs(filename = 'R_logs')```

To increase the log file limit, you can use ```max_log_file_size``` option

It can be added to Java cli: ```java -jar h2o.jar -max_log_file_size 128MB```

Or when launching Python: ```h2o.init(max_log_file_size="128MB")```

It doesn't seem to be available if launching in R, at the moment, but looking to add it.


## Getting Logs from H2O flow

On flow:

-the top where there is Admin button, 

-click the drop down, you can see view log or download log button

-download log option will downloads the zip file 

-however if downloading the log in zip is not an option click view logs option and copy paste it on text file or word 
