# IBM_Employee_Attrition-using-Hive-and-R
This project analyzes the IBM Employee Attrition dataset using Hive for data processing within the Hortonworks Sandbox, and R for visualization and insights. The goal is to explore factors influencing employee attrition and predict retention trends.

### Log into the Sandbox via SSH (or Web Client)
Access your sandbox system either via terminal or web-based SSH client (e.g., http://127.0.0.1:4200/).

### Upload Dataset to the Sandbox
First, upload your dataset to the sandbox using PSCP or any other preferred method (like scp).
Example command using pscp:
->(pscp -P 2222 "C:\path\to\dataset_IBM_HR_Data_new.csv" root@127.0.0.1:/root/)
Move the Dataset to HDFS

### After uploading, move the dataset to HDFS so it can be accessed by Hive.
1.Create Directory in HDFS:
->(hadoop fs -mkdir /user/root/hr_data)

2.Move the File to HDFS:
->(hadoop fs -put /root/dataset_IBM_HR_Data_new.csv /user/root/hr_data/)

3.Start Hive
Launch Hive to begin working with your data:
