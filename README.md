# Caterpillar-Inc.-Purdue_DataMine
## Advanced Detection of critical DiagnosticTroubleCodes(DTC)
**Problem Statement:**  <br /> 

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;    Caterpillar alertsmachine health and potential failure modesdirectlyto customers using DTC messageswith various severity levels usingmachineonboarddisplay. Note that ‘Severity level 3’ DTCs often requiresimmediate actionsby customers while ‘Severity level 1 and 2’DTCsdo not.Therefore, if we can establish a lead time relationship between ‘Severity level 1 and 2’ DTCs and ‘Severity level 3’ DTCs using machine learning, it will help alert customers in advance reducing unexpected downtime and/or prepare all required parts in advance. For this project, a set of ‘Severity level 3’DTC’s that resulted in immediate repairs by customers are selectedas ground truthfor a particular Caterpillar quarry truck sales model. Many more ‘Severity level 1 and 2’ DTCs will be provided as input, and the students are expected to develop a predictiveanalyticsmodel that can identify ‘Severity level 3’DTCsfrom ‘Severity level 1 and 2’DTCs in advance (e.g. minimal of 2 to 3 weeks)  

**Data:**  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;   Obfuscated DTCshistory for a group of quarry trucks(different severity and time stamps)Development  

**Environment:**  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Caterpillar AWS data scientist tenant with access to required data and SageMaker notebook

**Click on the image for a presentation video**

[![Advanced Detection of critical DiagnosticTroubleCodes(DTC)](https://i.postimg.cc/Qx2h00m9/Screenshot-1487.png)](https://www.youtube.com/watch?v=FeiPHIEMdUo&t=10s) 

## Multivariate_TimeSeries_MissingData_Imputation
**CAT 797F Monitoring Service:**  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Caterpillar provides condition monitoring services of machines to dealers and customers. The service includes alerting anomalies in machine sensors to dealers who will use them to create actionable recommendations for customers to follow on. Caterpillar data scientists leverage the machine sensor data to develop anomaly detection models, and one issue, sometimes, ran into is robustness of sensors that results in missing critical data for a period of time. In order to maintain high performance of the analytics models, we may have to fill the missing data gaps by imputing data.   


&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Caterpillar leverages continuous time series data at 1Htz frequency coming from machines to identify anomalies in machine health. Due to sensor failure and data pipeline network issues, sometimes, we observe missing data in one or more sensors for a time period, and this could result in poor performance of the analytics model. Machine learning (ML) models are trained using historical time series data from multiple sensors (5-20) and filling the missing data will be critical for developing a reliable ML model. For this project, a set of channels from a mining tuck(s) is selected and students are expected to impute the missing data that best represent expected behavior of the missing data channels.    

**Goal:** 

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Analytics model using Python used to fill the missing data, documented assumptions and limitations of the approaches, and cross validation results of the approach.  

**Data:**  
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; The data is obfuscated multi-month continuous time series data @1Hz frequency for a group of channels from a mining truck. It contains missing data in one or more channels for a time period. Datasets are stored in parquet format. There are 8 files per asset (one for each month), 76-78 channels per asset, with data recorded each second. Not all days and times are present. 
 
**Environment:**  

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; Data is stored on AWS in an S3 bucket. Data can be converted to a Pandas data frame or NumPy array for analysis. All work is done within Caterpillars AWS account, using Amazon Sagemaker.

**Click on the image for a presentation video**

[![Multivariate_TimeSeries_MissingData_Imputation](http://i3.ytimg.com/vi/2eRlcHS3bMU/maxresdefault.jpg)](https://www.youtube.com/watch?v=2eRlcHS3bMU)   

