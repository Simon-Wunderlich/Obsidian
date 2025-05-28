Created: May 28 2025
Class: [[SQL]] 
- - -
[[Wk9SQL]]

## Group by
Groups all rows of selected attribute sharing same value for GROUP BY value
```sql
SELECT * FROM
table1
GROUP BY attr1
```

### Aggregate functions
Can be used to aggregate attributes in the same group
```sql
COUNT(attr)
SUM(attr)
AVG(attr)
...
```

### Having
Where for aggregate functions
```sql
SELECT ... FROM ...
GROUP BY ...
HAVING {CONDITION};
```

## Set operators
### Union
Merge results of two tables
```sql
SELECT
...
UNION
SELECT
...
```
### Intersect
Select only shared values of two tables
```sql
SELECT
...
INTERSECT
SELECT
...
```

### Except
Select only values not shared between both tables
```sql
SELECT
...
MINUS
SELECT
...
```

## Views
Save results of queries to pseudo table
```sql
CREATE VIEW vName(vAttr1, vAtt2, ...) AS
SELECT attr1, attr2, ...
...
```
the vAttr's name the columns from the select statement
Querys can be run on views

## Insert data from other tables
```sql
INSERT INTO tabl2(vAttr1a, vAtt2a, ...)
SELECT attr1b, attr2b, ...
```

## Case
Change column based on condition
```sql
SELECT 
CASE
WHEN {condition} THEN attr1
WHEN {condition2} THEN attr2
ELSE attr3
END
FROM table;
```