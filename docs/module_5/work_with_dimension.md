# Work with dimensions

When you are building visuals, Power BI automatically enters values of the date type as a **hierarchy** (if the table has not been marked as a date table). Hierarchies allow you to view increasing levels of data on a single view.

The process of viewing multiple child levels based on a top-level parent is known as **flattening the hierarchy**. In this process, you are creating multiple columns in a table to show the hierarchical path of the parent to the child in the same record. You will use **PATH()** and **PATHITEM()**.

## Role-playing dimensions

Role-playing dimensions have multiple valid relationships with fact tables, meaning that the same dimension can be used to filter multiple columns or tables of data. As a result, you can filter data differently depending on what information you need to retrieve.