## Description
#### analyzeScript
`analyzeScript.java` decodes the SQL query into SQL identifier, constant, function, 
clauses and subquery according to the SQL grammar. 

This demo only illustrates how to decode some major SQL statements like select/update/insert/create table
/alter table/create view/create index/PLSQL create pacakge/MySQL create function/MySQL declare/return/if statements.
You may check [some sample result](http://sqlparser.com/decoding-sql-grammar.php) generated by this tool.

If you need to check how to iterate the parse tree node of all SQL statements in a generic way, 
please check [toXML demo](../visitors).

#### analyzePLSQLProcedure
`analyzePLSQLProcedure.java` illustrates how to get some basic information such as procedure name, parameters,
SQL statements used in the procedure body from an Oracle PLSQL code. 

#### iterateStatement
`iterateStatement.java` illustrates how to get select list/from clause/where clause/group by/order by clause
from the select statement.
 
#### tutorial
`tutorial.java` is a simple demo illustrates how to get union/minus/except/intersect operator and join condition
from the select statement.

## Usage
-  `java analyzeScript sqlfile.sql`
-  `java analyzePLSQLProcedure`
-  `java iterateStatement`
-  `java tutorial`

## Related demo
* [toXML demo](../visitors).

