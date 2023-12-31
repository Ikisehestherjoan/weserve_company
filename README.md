# weserve_company
WESERVE
PROBLEM STATEMENT:

WeServe operates as a call service agency that specializes in providing outsourced customer service personnel to multiple companies.
These customer service agents work from a centralized call center where they handle incoming and outgoing customer calls. 
Their primary responsibilities include addressing customer complaints and gathering feedback on products and services purchased from different companies.

All interactions with customers are documented and recorded in a call log sheet, with additional information being stored in a call details sheet.
To gain a deeper understanding of the call agents' activities, the customer service managers have made available a sample of these sheets for your analysis.

 Python was used in this project because it is a versatile programming language that can be used for a wide range of data engineering tasks, 
 from data integration and transformation to ETL (Extract, Transform, Load) processes, data modeling, and more. It can also be used for merging datas, 
 data analysis, and visualization, making it a one-stop solution for various data-related tasks.Moreover the dataset is relatively smaller in size

TOOLS USED.

PYTHON

PANDAS

PSYCOPG2

SQLALCHEMY

MATPLOTLIB

SEABORN


Warehouse schema (structure) 

INITIAL SCHEMA FOR CALL DETAILS

<class 'pandas.core.frame.DataFrame'>

RangeIndex: 600 entries, 0 to 599

Data columns (total 5 columns):

 #Column                 Non-Null Count  Dtype 
 
---  ------                 --------------  ----- 

 0   callID                 600 non-null    object
 
 1   callDurationInSeconds  600 non-null    int64 
 
 2   agentsGradeLevel       600 non-null    object
 
 3   callType               600 non-null    object
 
 4   callEndedByAgent       600 non-null    bool


 INITTIAL SCHEMA FOR CALL LOGS
 
 <class 'pandas.core.frame.DataFrame'>
 
RangeIndex: 600 entries, 0 to 599

Data columns (total 7 columns):

 # Column                     Non-Null Count  Dtype  
 
---  ------                     --------------  -----  

 0   id                         600 non-null    int64  
 
 1   callerID                   600 non-null    object 
 
 2   agentID                    600 non-null    int64  
 
 3   complaintTopic             600 non-null    object 
 
 4   assignedTo                 372 non-null    float64
 
 5   status                     600 non-null    object 
 
 6   resolutionDurationInHours  187 non-null    float64



MERGED_DATA_SET
<class 'pandas.core.frame.DataFrame'>

Int64Index: 600 entries, 1 to 600

Data columns (total 10 columns):

 #Column                     Non-Null Count  Dtype  
---  ------                     --------------  -----  

 0   callerID                   600 non-null    object 
 
 1   agentID                    600 non-null    int64 
 
 2   complaintTopic             600 non-null    object 
 
 3   assignedTo                 600 non-null    float64
 
 4   status                     600 non-null    object 
 
 5   resolutionDurationInHours  600 non-null    int32  
 
 6   callDurationInSeconds      600 non-null    int64  
 
 7   agentsGradeLevel           600 non-null    object 
 
 8   callType                   600 non-null    object 
 
 9   callEndedByAgent           600 non-null    bool 

STEPS AND PROCESSES TAKEN

Data Collection:

Gather call data from various sources, including call logs and call details sheets, which may be stored in different formats or databases.

Data Integration:

Use Python libraries like Pandas and NumPy to integrate, clean, and preprocess data. For instance, you can read data from Excel files, CSV, or databases and 

merge them into a single, unified dataset.

Data Transformation:

Apply data transformation techniques in Python to handle missing values, standardize data formats, and ensure data quality. This includeS filtering, aggregating,

and sorting data.

Data Storage:

Design and manage data storage solutions using Python and libraries

ETL Processes:

Develop and maintain ETL (Extract, Transform, Load) pipelines using Python to automate the movement of data from source systems to a data base

SOME KPI USE CASE 

- Total Number of Calls Resolved vs Total Number of Calls Received
 
- Total Number of calls received vs Total Number of calls assigned/resolved
 
- The total and average call duration for each agent, and the grade level of these agents.
 
- The earliest and latest closed and resolved calls, and the grade levels of the agents who resolved these cases etc
  










