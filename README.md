# SQL-SERVER

<h3>BASIC</h3>

Variables: placeholder for a specific value of a specific data type.
DECLARE @varname datatype
Assigning Value to variables: SET @varname = / SELECT @varname = 
Show Value: SELECT @varname

<b>DATA TYPE CONVERSION</b>
CAST() comes from SQL standard.
CONVERT() is specific to SQL Server

TOP(N): Returns Top N records.
TOP(N) PERCENT: Returns Top N% of records.

AS Keyword: Used for providing alias names to columns and tables for query results.

Range: BETWEEN, NOT BETWEEN, IN, NOT IN, <>

Boolean: AND, OR

---------------------------------------------------------------------------------------------------------------------------------
<h3>STRING MANIPULATION</h3>

LIKE, NOT LIKE
Beginning with 'A%', Ending with '%a'

LEN(COL)
LEFT(COL,NUM)
RIGHT(COL,NUM)

CHARINDEX(CHAR,COL)
PATINDEX(PATTERN,COL)
SUBSTRING(COL,START,NUM)
REPLACE(COL,FIND_CHAR,REPLACE_CHAR)

----------------------------------------------------------------------------------------------------------------------------------
<h3>EDA using T-SQL</h3>

L1: Exploring data with aggregation - Summary Statistics
    MIN,MAX,AVG,SUM,COUNT

Detecting missing values use IS NULL, IS NOT NULL
There is a difference between blank value('') and a NULL value.
Blank values can be avoided in result by using LEN(field) > 0

To substitute missing data with a specific value use ISNULL() or COALESCE() function.

ISNULL(field,substituted value/field)
COALESCE(val1,val2,...valn), returns the first non-missing value.

Binding data with CASE statement
Four mandatory keywords - CASE WHEN THEN END

ABS() - Absolute
SQRT() - Square Root
SQUARE() - Square
LOG(col,baseval) - logs, logarithm value 

WHILE LOOPS

<b>Common Window Functions</b>
Seeing end results of aggregation without changing the grain of data.

FIRST_VALUE() - returns the first value in the window requires ORDER BY clause
LAST_VALUE() - returns the last value in the window requires ORDER BY clause
LEAD() - next row value requires ORDER BY clause
LAG() - previous row value requires ORDER BY clause
ROW_NUMBER() - sequentially numbers the rows in the window. Requires ORDER BY clause

<b>Temporary Tables</b>
Temporary tables exist until connections/sessions end.

SELECT col1,col2
INTO #temp_table
FROM table

DROP TABLE #temp_table
--------------------------------------------------------------------------------------------------------------------------------------

<h3>Time Series Analysis</h3>
Refer the folder


