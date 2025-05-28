Created: May 28 2025
Class: [[SQL]] 
- - -
[[Wk9SQL]]

### Group by
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

### Union
Merge results of two tables
```sql
SELECT
...
UNION
SELECT
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

### Minus  / Except
Select only values not shared between both tables
```sql
SELECT
...
MINUS
SELECT
...
```

