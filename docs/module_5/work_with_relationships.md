# Work with relationships and cardinality

Unlike other database management systems, Power BI has the concept of directionality to a relationship. This directionality plays an important role in filtering data between multiple tables.

## Relationships

**Many-to-one (\*:1)** or **one-to-many (1:\*)** relationship:
- it describes a relationship in which you have many instances of a value in one column that are related to only one unique corresponding instance in another column
- it describes the **directionality** between fact and dimension tables
- it is the most common type of directionality and is the **Power BI default** when you are automatically creating relationships

**One-to-one (1:1)** relationship:
- it describes a relationship in which only one instance of a value is common between two tables
- it requires unique values in both tables.
- it is not recommended because this relationship stores redundant information and suggests that the model is not designed correctly
- it is **better practice to combine the tables**

**Many-to-many (\*.\*)** relationship:
- it describes a relationship where many values are in common between two tables
- it does not require unique values in either table in a relationship
- **it is not recommended**: a lack of unique values introduces ambiguity and your users might not know which column of values is referring to what

## Cross-filter direction

Data can be filtered on one or both sides of a relationship.

With a single **cross-filter direction**:
- only one table in a relationship can be used to filter the data
- for a one-to-many or many-to-one relationship, the cross-filter direction will be from the "one" side, meaning that the filtering will occur in the table that has many values.

**NOTE.** Follow the direction of the arrow on the relationship between your tables to know which direction the filter will flow. **You typically want these arrows to point to your fact table.**

With both cross-filter directions or bi-directional cross-filtering:
- one table in a relationship can be used to filter the other
- you might have lower performance when using bi-directional cross-filtering with many-to-many relationships

**NOTE.** You should not enable bi-directional cross-filtering relationships unless you fully understand the ramifications of doing so. Enabling it can lead to ambiguity, over-sampling, unexpected results, and potential performance degradation.