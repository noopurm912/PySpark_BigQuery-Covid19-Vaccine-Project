# PySpark_BigQuery-Covid19-Vaccine-Project
COVID-19 Vaccine Analaysis using SparkSQL and bigQuery on Google Cloud Platform<br>
The project aims to analyze the distribution of COVID-19 vaccination globally and present the overall progress of vaccination around the world.<br>
•	The main objectives of the project will be focusing on vaccination progress for each country for example, which country is providing maximum vaccination to their people. <br>
•	We will analyze that how many people got fully vaccinated versus the total number of people who got vaccinated because some vaccines require two doses. <br>
•	We will study the vaccine distribution on a monthly as well as yearly basis and analysis of vaccines used by the different countries.

<h4>Data Source<h4>
The dataset is acquired from Kaggle. It included COVID-19 world vaccination progress. The data is regularly maintained and updated. we have worked on the dataset which is updated till 6th April. Link: https://www.kaggle.com/gpreda/covid-world-vaccination-progress.<br>

 <h4>Architecture & Implementation</h4>
  
We used Google Cloud Platform for the implementation of the project.<br>
•	First, ingested the dataset to google cloud storage. <br>
•	Used cloud Dataproc to implement the spark project, ceated a cluster in Dataproc with three worker nodes and one master node. <br>
•	Created a pyspark jupyter notebook in the cluster and read the dataset from cloud storage and dataproc enables the use of cloud storage in parallel with HDFS. <br>
•	PySpark SQL is used to query the data and saving the results to cloud storage. <br>
•	The results are later saved in the google BigQuery tables to enable the connection with Tableau online for data visualization.<br>
