# Reading Notes 08

## SQL

SQL stands for structured query language. The language was designed with simplicity in mind so that its use could wide-reaching. It allows a user to manipulate data inside of a realational database. A relational database is essentially a collection of two-dimensional tables. The columns are defined and set, but it can have any number of rows of stored data.

### Basic Commands

- SELECT - chooses info from specified columns
- WHERE - sets of a conditional of your choice (some conditionals are written in english words)
- DISTINCT - blindly removes duplicate rows
- ORDER BY - orders results by a specification (ASC or DESC)
- INSERT INTO - addes new rows with information
- UPDATE ... SET - allows rows that have already been made to be changed in place
- DELETE FROM - allows rows to be deleted
- **NOTE** - it is recommended to first run a SELECT on rows you want to UPDATE or DELETE to ensure it is what you were expecting before going through with the irreversable function.

### Tables

- CREATE TABLE IF NOT EXISTS - will create a new table chekcing if one with the same name exists or not
- **NOTE** - tables are made from schema which declare the name of columns, the data type of the column, and optionally the constraint of the column input
- ALTER TABLE - preps command for which table will be altered
- ADD - used to add a new column with the same specifications used when creating a full table
- DROP - removes a column of data from a table
- RENAME TO - renames a table something else
- DROP TABLE IF EXISTS - completely deletes a table. This does not just delete all of the rows, but deletes it in its entirety including whatever schema it had



#### [Home](README.md)