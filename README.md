#  Cloud Project

This project implements a cloud-based distributed data processing system using **Apache Spark** to analyze a large-scale taxi trip dataset.  
The main objective of the project is to study Spark’s scalability behavior and performance when running with different numbers of workers using local[N] mode.


##  Project Objectives
 Apply distributed data processing concepts using Apache Spark.
 Perform descriptive statistics and MapReduce-style aggregation.
 Execute multiple machine learning tasks using Spark MLlib.
 Measure execution time, speedup, and efficiency for different cluster  sizes.
 Analyze scalability behavior under limited hardware resources.


##  Dataset
 Type: CSV file  
 Data:Taxi trip records including trip distance, fare amount, pickup and drop-off locations.  
The dataset is uploaded directly by the user through Google Colab.


##  System Workflow
1. The user uploads a CSV file using the Google Colab interface.
2. A Spark session is created in local[N] mode.
3. The dataset is loaded into a Spark DataFrame.
4. Descriptive statistics are computed.
5. A MapReduce aggregation task is executed.
6. Machine learning models are trained and evaluated.
7. Performance metrics are calculated and displayed.


##  Machine Learning Tasks
The following machine learning jobs are implemented using Spark MLlib:
1. **KMeans Clustering** with Silhouette evaluation.
2. **Linear Regression** for fare amount prediction.
3. **Random Forest Regression** for fare amount prediction.
4. **FPGrowth** for frequent itemset mining.


##  Performance Evaluation
 The same MapReduce workload is executed using:
   1 Nodes 
   2 Nodes 
   4 Nodes 
   8 Nodes 
Execution time is recorded for each configuration.
Speedup and efficiency are calculated based on the execution time of 1 Node.
Results are displayed in a structured performance table.


##  Cloud Deployment
 The project is executed on Google Colab.
Spark runs in `local[N]` mode to simulate a distributed cluster.
 All processing and results are displayed directly on the cloud platform.
 
## Repository Structure

spark-taxi-cloud-project/
│
├── README.md
├── src/
│   └── Project.ipynb
└── report/
    └── projectReportTemplate-2026.pdf

 


## Project Links
Google Colab Notebook:
  https://colab.research.google.com/drive/1SGGSaSuOu19xS_3K2R17E84vOGWTyNSn?usp=sharing

GitHub Repository:
  https://github.com/Abd-Elrahman-Jehad/spark-taxi-cloud-project.git

Video Demonstration: 
  https://youtu.be/Q3zemq1KLJ0


##  Conclusion
This project demonstrates how Apache Spark can be used to perform distributed data processing and machine learning tasks in a cloud environment. The results show that increasing the number of Nodes improves performance up to a certain point, after which system overhead and resource limitations reduce efficiency. The project provides practical insight into Spark’s scalability behavior under constrained environments.
