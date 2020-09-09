# SQL-SERVER

<h3>BASIC</h3>

Variables: placeholder for a specific value of a specific data type.<br>
DECLARE @varname datatype<br>
Assigning Value to variables: SET @varname = / SELECT @varname = <br>
Show Value: SELECT @varname<br>

<b>DATA TYPE CONVERSION</b><br>
CAST() comes from SQL standard.<br>
CONVERT() is specific to SQL Server<br>

TOP(N): Returns Top N records.<br>
TOP(N) PERCENT: Returns Top N% of records.<br>

AS Keyword: Used for providing alias names to columns and tables for query results.<br>

Range: BETWEEN, NOT BETWEEN, IN, NOT IN, <><br>

Boolean: AND, OR<br>

---------------------------------------------------------------------------------------------------------------------------------
<h3>STRING MANIPULATION</h3>

LIKE, NOT LIKE<br>
Beginning with 'A%', Ending with '%a'<br>

LEN(COL)<br>
LEFT(COL,NUM)<br>
RIGHT(COL,NUM)<br>

CHARINDEX(CHAR,COL)<br>
PATINDEX(PATTERN,COL)<br>
SUBSTRING(COL,START,NUM)<br>
REPLACE(COL,FIND_CHAR,REPLACE_CHAR)<br>

----------------------------------------------------------------------------------------------------------------------------------
<h3>EDA using T-SQL</h3>

L1: Exploring data with aggregation - Summary Statistics<br>
    MIN,MAX,AVG,SUM,COUNT<br>

Detecting missing values use IS NULL, IS NOT NULL<br>
There is a difference between blank value('') and a NULL value.<br>
Blank values can be avoided in result by using LEN(field) > 0<br>

To substitute missing data with a specific value use ISNULL() or COALESCE() function.<br>

ISNULL(field,substituted value/field)<br>
COALESCE(val1,val2,...valn), returns the first non-missing value.<br>

Binding data with CASE statement<br>
Four mandatory keywords - CASE WHEN THEN END<br>

ABS() - Absolute<br>
SQRT() - Square Root<br>
SQUARE() - Square<br>
LOG(col,baseval) - logs, logarithm value <br>

WHILE LOOPS<br>

<b>Common Window Functions</b><br>
Seeing end results of aggregation without changing the grain of data.<br>

FIRST_VALUE() - returns the first value in the window requires ORDER BY clause<br>
LAST_VALUE() - returns the last value in the window requires ORDER BY clause<br>
LEAD() - next row value requires ORDER BY clause<br>
LAG() - previous row value requires ORDER BY clause<br>
ROW_NUMBER() - sequentially numbers the rows in the window. Requires ORDER BY clause<br>

<b>Temporary Tables</b><br>
Temporary tables exist until connections/sessions end.<br>

SELECT col1,col2<br>
INTO #temp_table<br>
FROM table<br>

DROP TABLE #temp_table<br>

--------------------------------------------------------------------------------------------------------------------------------------
<h3>Time Series Analysis</h3>
Refer the folder


