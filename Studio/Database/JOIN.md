Created: May 21 2025
Class: [[SQL]] 
- - -
Joins two tables together
## Inner join
Default
Includes rows from both tables where the condition is met

``` sql
SELECT l.attr, r.attr
	FROM left_table as l
	JOIN right_table as r ON {condition};
```

## Outer join
### Left outer join
Includes all rows where condition is met plus all rows from left table where condition is not met
``` sql
SELECT l.attr, r.attr
	FROM left_table as l
	LEFT JOIN right_table as r ON {condition};
```
### Right outer join
Less common - Can be re-written as left join
Includes all rows where condition is met plus all rows from right table where condition is not met
### Full outer join
Includes all rows from both tables

## Joining 3 or more tables
``` sql
SELECT one.attr, two.attr, three.attr
	FROM table1 as one
	JOIN table2 as two ON {condition}
	JOIN table3 as three ON {condition};
```

## Natural Join
If two tables have the same named attribute, (ie foreign key) u can use NATURAL JOIN to join them
``` sql
SELECT l.attr, r.attr
FROM left_table as l
NATURAL JOIN right_table as r;
```

## Sub-queries
You can nest separate queries within a WHERE statement
If attr from table 1 is in the resultant row from the sub query, it is outputted
``` sql
SELECT attr
FROM table1
WHERE attr IN (SELECT attr FROM table2 WHERE table1.attr = table2.attr)
```

## Exists
If the subquery returns any rows, the outer query returns a row
```sql
SELECT attr
FROM table1
WHERE EXISTS (
	SELECT 1
	FROM table2
	WHERE table1.attr = table2.attr
)
```

## Avoid aggregate function missue
```sql
SELECT attr1, attr2
FROM table1
WHERE attr2 IN (
	SELECT MAX(attr2) FROM table2
);
```
