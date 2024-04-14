# Semantic Model

A good **semantic model** offers the following benefits:
- data exploration is faster
- aggregations are simpler to build
- reports are more accurate
- writing reports takes less time
- reports are easier to maintain in the future

Generally, a smaller semantic model is better because it performs faster and will be simpler to use.

Typically, a smaller semantic model is composed of fewer tables and fewer columns in each table that the user can see. Collapsing tables make the semantic model more intuitive to the user. Removing unneeded columns increases the likelihood that the user reads all column names. 

Power BI allows relationships to be built from tables with different data sources, a powerful function that enables you to pull one table from Microsoft Excel and another from a relational database. You would then create the relationship between those two tables and treat them as a unified semantic model.

## Star Schemas

In a star schema, each table within your semantic model is defined as a **dimension** or a **fact** table.

Fact tables contain observational or event data values: sales orders, product counts, prices, transactional dates and times, and quantities. Fact tables can contain several repeated values. For example, one product can appear multiple times in multiple rows, for different customers on different dates. These values can be aggregated to create visuals. For instance, a visual of the total sales orders is an aggregation of all sales orders in the fact table. With fact tables, it is common to see columns that are filled with numbers and dates. The numbers can be units of measurement, such as sale amount, or they can be keys, such as a customer ID. The dates represent time that is being recorded, like order date or shipped date.

Dimension tables contain the details about the data in fact tables: products, locations, employees, and order types. These tables are connected to the fact table through key columns. Dimension tables are used to filter and group the data in fact tables. The fact tables, on the other hand, contain the measurable data, such as sales and revenue, and each row represents a unique combination of values from the dimension tables. For the total sales orders visual, you could group the data so that you see total sales orders by product, in which product is data in the dimension table.

Fact tables are much larger than dimension tables because numerous events occur in fact tables, such as individual sales. Dimension tables are typically smaller because you are limited to the number of items that you can filter and group on. For instance, a year contains only so many months, and the United States are composed of only a certain number of states.