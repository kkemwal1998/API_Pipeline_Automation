# Project Name : API Pipeline Automation

# Technology: Azure Data Factory

# API Source: https://www.data.govt.nz/catalogue-guide/using-data-govt-nz-apis

# Objective: To extract information from an API using Azure Data Factory (ADF) and load it into SQL Server Management Studio (SSMS), you can follow these steps

# Procedures:

# 1. Set up the API Integration in Azure Data Factory:

  - In Azure Data Factory (ADF), navigate to Linked Services and create a new Linked Service.

  - Select the REST or HTTP connector, depending on the API type.

  - Provide the necessary information such as API endpoint, authentication type (basic, OAuth, etc.), and credentials if needed.

# 2. Create a Pipeline in ADF:

  - In ADF, go to the Author tab and create a new pipeline.

  - Drag and drop the Copy Data activity into the pipeline. This activity will be responsible for extracting data from the API and writing it to a sink.

  - In the Source tab of the Copy Data activity, configure it to use the REST or HTTP Linked Service you created earlier.

  - Set the request Request and POST type.

# 3. Create a Linked Service for SQL Server:

  - In Linked Services, create another new Linked Service for SQL Server.

  - Provide the SQL Server name, database, credentials, and connection details

# 4. Configure Sink in ADF

  - In the Sink tab of the Copy Data activity, choose the Linked Service for SQL Server

  - Define the target table where you want to load the data from the API. You can create a new table if needed or append to an existing one.

# 5. Pipeline Automation:

  - You can run the pipeline on-demand or set up a scheduled trigger based on your requirements.

 
