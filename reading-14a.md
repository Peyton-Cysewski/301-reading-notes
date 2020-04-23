# Reading Notes 14a

## Normalization
Normalizing a database minimizes duplicate data, minimizes or avoids data modification issues, and makes queries easier overall. Whenever there are sets of duplicated data, by happenstance or purposefully, updating all of those pieces of the same data can lead to anomalies. This is because if even on of those instances is left unchanged, undeleted, or inserted improperly, then it creates a massive problem for data consistency and continuity. Data that is necessarily duplicated should just land in a table all on its own. This can make certain queries like ones that may require multiple `UNION`'s or column searches return to the form of a simple one-liner. All of this thought can be summed into three main points:
- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.
- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key



#### [Home](README.md)