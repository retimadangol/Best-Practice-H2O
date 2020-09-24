Below are methods that could download logs for Python or R code.

Python:
h2o.download_all_logs('logs_in_Py')

R:
h2o.downloadAllLogs(filename = 'R_logs')

Based on our conversation today, it sounds like we should increase the log file limit. As mentioned in the section for starting H2O, you can use 'max_log_file_size'.
It can be added to Java cli: java -jar h2o.jar -max_log_file_size 128MB
Or when launching Python: h2o.init(max_log_file_size="128MB")
It doesn't seem to be available if launching in R, at the moment, but looking to add it.
