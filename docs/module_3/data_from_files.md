# Get data from files

Organizations often export and store data in files. 

One possible file format is a flat file. A flat file is a type of file that has only one data table and every row of data is in the same structure. The file doesn't contain hierarchies. Likely, you're familiar with the most common types of flat files, which are comma-separated values (.csv) files, delimited text (.txt) files, and fixed width files. 

Another type of file would be the output files from different applications, like Microsoft Excel workbooks (.xlsx).

## Connect to data in a file

Power BI Desktop allows you to get data from many types of files. 

The first step is to determine which file location you want to use to export and store your data.

Your file might exist in one of the following locations:
- **Local**
    - You can import data from a local file into Power BI
    - The file isn't moved into Power BI and a link doesn't remain to it
    - A new semantic model is created in Power BI and data from the Excel file is loaded into it
    - Changes to the original Excel file aren't reflected in your Power BI semantic model
    - You can use local data import for **data that doesn't change**
- **OneDrive**
    - You can pull data from OneDrive into Power BI
    - This method is effective in keeping an Excel file and your semantic model, reports, and dashboards **synchronized**
- **SharePoint - Team Sites**
    - Saving your Power BI Desktop files to SharePoint Team Sites is similar to saving to OneDrive
