# Get data from Azure Analysis Services

**Azure Analysis Services** is a fully managed platform as a service (PaaS) that provides enterprise-grade semantic models in the cloud. 

You can use advanced mashup and modeling features to combine data from multiple data sources, define metrics, and secure your data in a single, trusted tabular semantic model. The semantic model provides an easier and faster way for users to perform ad hoc data analysis using tools like Power BI.

Getting data from Azure Analysis Services server is similar to getting data from SQL Server, in that you can:
- Authenticate to the server
- Pick the model you want to use
- Select which tables you need

Notable differences between Azure Analysis Services and SQL Server are:
- Analysis Services models have calculations already created
- If you don’t need an entire table, you can query the data directly
- Instead of using Transact-SQL (T-SQL) to query the data, like you would in SQL Server, you can use **multi-dimensional expressions** (MDX) or **data analysis expressions** (DAX)

## Connect to data in Azure Analysis Services 

**Connect live** is an option for Azure Analysis Services. Azure Analysis Services uses the tabular model and DAX to build calculations, similar to Power BI. These models are compatible with one another. Using the Connect live option helps you keep the data and DAX calculations in their original location, without having to import them all into Power BI. 

Azure Analysis Services can have a **fast refresh schedule**, which means that when data is refreshed in the service, Power BI reports will immediately be updated, without the need to initiate a Power BI refresh schedule. This process can improve the timeliness of the data in your report.

Similar to a relational database, you can choose the tables that you want to use. If you want to directly query the Azure Analysis Services model, you can use DAX or MDX.

NOTE. You'll likely import the data directly into Power BI. An acceptable alternative is to import all other data that you want (from Excel, SQL Server, and so on) into the Azure Analysis Services model and then use a live connection. This approach simplifies your solution by keeping the semantic modeling and DAX measures in one place.
