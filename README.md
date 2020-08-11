# Visualize Parquet Tool
A simple Databricks dashboard for visualizing your parquet data's distribution and statistics.

## How-To

1. Import the notebook (.dbc) into your Databricks workspace.

2. Open the notebook **Utils_VisualizeParquet**

3. Switch to **Dashboard View**
<img src="https://jixjiastorage.blob.core.windows.net/blog-resources/10x-spark-performance/dashboard_view.png">

4. Add your **Root Path of Parquet** to the widget, and hit **Update** button
<img src="https://jixjiastorage.blob.core.windows.net/blog-resources/10x-spark-performance/dashboard.gif">


## Dashboard
You'll get following information from the dashboard:

(1) Total Size - total dataset size   
(2) Total Files - number of files in a parquet path   
(3) Avg File Size - average file size   
(4) Total Partitions - number of disk partitions (=1 if not partitioned)   
(5) Avg Partition Size - average size of each disk partition   
(6) Files Per Partitions - average number of files in each disk partition   
(7) Statistics - descriptive stats of disk partitions and its size   
(8) Partition Size Graph - graph showing the partition size in a descending order. Useful for checking partition skewness   
(9) Num Files Graph - graph showing number of files in each partition. Useful for checking if executors are fully utilized for each partition   

<img src="https://jixjiastorage.blob.core.windows.net/blog-resources/10x-spark-performance/dashboard_explain.gif">
