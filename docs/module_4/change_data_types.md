# Evaluate and change column data types

When you import a table from any data source, Power BI Desktop automatically starts scanning the first 1K rows (default setting) and tries to detect the type of data in the columns. 

Some situations might occur where Power BI Desktop doesn't detect the correct data type.

A best practice is to evaluate the column data types in Power Query Editor **before you load the data** into a Power BI semantic model. If you determine that a data type is incorrect, you can change it. You might also want to apply a format to the values in a column and change the summarization default for a column.

## Implications of incorrect data types

Incorrect data types will prevent you from creating certain calculations, deriving hierarchies, or creating proper relationships with other tables. 

For example, if you try to calculate the *Quantity of Orders YTD*, you'll get the following error stating that the *OrderDate* column data type isn't *Date*, which is required in time-based calculations. Another issue with having an incorrect data type applied on a date field is the inability to create a date hierarchy, which would allow you to analyze your data on a yearly, monthly, or weekly basis. 


