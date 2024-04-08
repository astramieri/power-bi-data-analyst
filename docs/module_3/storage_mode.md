# Select a storage mode

The most popular way to use data in Power BI is to **import it** into a Power BI semantic model. Importing the data means that the data is stored in the Power BI file and gets published along with the Power BI reports. This process helps make it easier for you to interact directly with your data. However, this approach might not work for all organizations.

However, sometimes there may be security requirements around your data that make it impossible to directly import a copy. Or your semantic models may simply be too large and would take too long to load into Power BI, and you want to avoid creating a performance bottleneck. Power BI solves these problems by using the **DirectQuery** storage mode, which allows you to query the data in the data source directly and not import a copy into Power BI. DirectQuery is useful because it ensures you're always viewing the most recent version of the data.

The three different types of storage modes you can choose from:
- **Import**
    - It allows you to create a **local copy** of your semantic models from your data source
    - You can use all Power BI service features with this storage mode, including Q&A and Quick Insights
    - Data refreshes can be scheduled or on-demand
    - Import mode is the **default** for creating new Power BI reports
- **DirectQuery**
    - The required data will be retrieved from the underlying data source (data won't be cached)
    - Using this model ensures that you're always viewing the most up-to-date data, and that all security requirements are satisfied
    - This mode is suited for when you have **large semantic models** to pull data from
- **Dual (Composite mode)**
    - You can identify some data to be directly imported and other data that must be queried
    - Any table that is brought in to your report is a product of both Import and DirectQuery modes
    - Using the Dual mode allows Power BI to choose the most efficient form of data retrieval