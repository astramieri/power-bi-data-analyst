# Resolve data import errors

The following sections cover some of the more common error messages that you might encounter in Power BI.

## Query timeout expired

Some relational systems and their administrators seek to limit a user from monopolizing all hardware resources by setting a query timeout. These timeouts can be configured for any timespan, from as little as five seconds to as much as 30 minutes or more.

## Power BI Query Error: Timeout expired

This error indicates that you’ve pulled too much data according to your organization’s policies. Administrators incorporate this policy to avoid slowing down a different application or suite of applications that might also be using that database.

NOTE. If you need the rows, columns, and complexity, consider taking small chunks of data and then bringing them back together by using Power Query. For instance, you can combine half the columns in one query and the other half in a different query. Power Query can merge those two queries back together after you're finished.

## We couldn't find any data formatted as a table

Power BI expects to find data formatted as a table from Excel.

## Couldn't find file

Usually, this error is caused by the file moving locations or the permissions to the file changing. If the cause is the former, you need to find the file and change the source settings.

## Data type errors

Sometimes, when you import data into Power BI, the columns appear blank. This situation happens because of an error in interpreting the data type in Power BI. The resolution to this error is unique to the data source. 