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