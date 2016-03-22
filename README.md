<h2>About</h2>

The State of Connecticut implemented changes to the Alvin W. Penn. Act to prohibit racial profiling of subjects at traffic stops. This dataset is the first analysis after the changes to the act were implemented in the year 2013. The dataset is extarcted from https://www.data.gov. We will be processing the data on Hadoop Cluster using HiveQL. The final output would be demonstrated with the help of Power BI and Tableau.

<h3>System Requirements</h3>

<b>Number of worker nodes-</b>4

<b>Memory Size:</b> 605GB(Worker node) & 285GB(Head node)

<b>CPU/core speed:</b> 56GHz(Worker node) & 7GHz(Head node)

<h3>Getting Started</h3>

<h3>Step 1</h3>

<h4>Creating an Azure Storage Account and provision a Hadoop Cluster.</h4>

NOTE: Before starting the process you should have

MS Azure subscription – you can get a free trial version from Get Azure free trial.
Workstation Computer – You should have a computer with Microsoft Excel 2013/MS Office 2013 Professional Plus/Office 2010 Pro Plus.
By default an HDInsight Cluster on Hadoop is provisioned in the same data centre as the specified Azure Storage account.

<b>Step 1.1:</b> You should sign in to the Azure Portal.

<b>Step 1.2:</b> Click NEW in the lower-left corner and then enter the necessary values.

<h4>Creating Storage Account</h4>

NOTE: Make sure that the storage account is created in a location that is supported for the cluster i.e. East Asia, Southeast Asia, North Europe, West Europe, East US, West US, North Central US, South Central US.

<b>Step 1.3:</b> Select the new storage account form the list and click MANAGE ACCESS KEYS at the bottom of the page to make a note of PRIMARY ACCESS KEY/SECONDARY ACCESS KEY.

A Hadoop cluster can be created by using Azure Portal, HDInsight .NET SDK Follow the following steps to create the Cluster

<b>Step 1.4:</b> Sign in to Azure Portal.

<b>Step 1.5:</b> Click on NEW in lower-left corner and then enter values as shown in image.

<h4>Hadoop Cluster</h4>

Click cluster name where you want to run the sample to Run the sample form Azure Portal -> click Query Console at the bottom -> click Getting Started Gallery tab -> under Samples category click the sample you want to run

<h3>Step 2</h3>

<h4>Uploading dataset to Microsoft Azure Blob Storage using Azure Management Studio</h4>

<b>Step 2.1:</b> Open Azure Management Studio and follow the steps

-> Goto Storage Accounts -> Blob Containers (your created folder here racial) -->Select the file from your local system (here it is cis520data CSV file)

<h3>Step 3</h3>

Verify the data to Azure Blob storage using Microsoft Azure HDInsight Query Console

<b>Step3.1:</b> Login into Microsoft Azure HDInsight QUERY CONSOLE

<b>Step3.2:</b> Once the HDInsight Cluster is provisioned in the Azure portal, click on the cluster name where you want to run the query.

<b>Step 3.3:</b> Enter the Hadoop user account and password. The default user name is admin; the password is what you entered while provisioning the cluster.

<b>Step 3.4:</b> Navigate to File Browser in order to view the uploaded file.

<h3>Step 4</h3>

<h4>Hive Queries</h4>

<b>Step 4.1:</b> Performing the Hive queries Goto Hive Editor in Microsoft Azure HDInsight Query Console.

<b>Step 4.2:</b> On the Hive Editor tab, for Query Name, enter Q1. The query name is the job title.

<b>Step 4.3:</b> In the query pane, enter the Hive queries one by one as mentioned in the file "HiveQL Queries.txt".

<b>Step 4.4:</b> Click Submit. It takes a few moments to get the results back.

<b>Step 4.5:</b> When the Status field changes to Completed, select View Details for the job. On the details page, the Job Output would be displayed.

<b>Step 4.6:</b> The output of the queries can also be saved in the local machines as .csv files.

[Note: "HiveQL Queries.txt" contains the list of queries executed in this application.All the queries can be executed in the similar manner as described above]

<h3>Step 5</h3>

<h4>Exporting data to Visualize outputs</h4>

NOTE: The output files were saved as .csv files which were then used as input to Tableau and Power BI for the purpose of making attractive dashboards.

<b>Step5.1:</b> Drag and drop the necessary output files to the Tableau and Power BI Desktop Apps respectively.

<b>Step5.2:</b> From the required output files, choose the necessary attributes for the reporting.

<b>Step5.3:</b> In Power BI, choose the type of visual tool you'd like your data to be displayed in.

<b>Step5.4:</b> Then, choose the Axis, Legend and Value fields from the respective .csv file.



Special Thanks

(https://github.com/) GitHub for API and UI</br>
Microsoft Azure</br>
Microsoft Excel</br>
Power BI</br>
Tableau</br>
</br>
<h4>Developed by :</h4>

JYOTI PATI</br>
RAVI BHADANA</br>
KRISHNA MARVANIYA
