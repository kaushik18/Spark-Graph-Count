This project utilizes the spark GraphX to:
	construct a graph of the votes of wiki pages
        find out the various metrics for each of the nodes of the graph. 

Tools: IntelliJ IDEA, AWS EMR Cluster

Steps for implementing the project : 

1.	Open AWS Elastic Map Reduce (EMR) and create a cluster containing Hadoop and spark. emr5.31 is preferred. 
2.	Go to steps and click on add a step.
3.	Following are the arguments : 

spark-submit --deploy-mode cluster --class WikiGraph --jars s3://assignment2/graphframes-0.8.1-spark2.4-s_2.11.jar s3://assignment2/kafka_2.11-0.1.jar s3://assignment2/wiki-Vote.txt s3://assignment2/Assign3

Spark file : s3://assignment2/kafka_2.11-0.1.jar
Spark Arguments : s3://assignment2/wiki-Vote.txt
s3://assignment2/Assign3




