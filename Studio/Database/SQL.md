Created: May 14 2025
Class: [[Database]]
- - -
Use \" for labels 
``` sql
SELECT name AS "USERNAME";
```
User \' for string literals
```sql
SELECT * 
FROM table
WHERE name == 'exampleName';
```

### Like keyword
#### Wildcards
- % - Represents zero, one, or multiple characters
- _ - Represents a single character (MS Access uses a question mark (?) instead)

Eg
``` sql
-- Selects all elements whose names end with hi
SELECT * 
FROM table
WHERE name LIKE 'hi';

-- Selects all elements with hi anywhere in their names
SELECT *
FROM table 
WHERE name LIKE '%hi%';

-- Selects all elements whose names have exactly 3 characters before hi
SELECT *
FROM table
WHERE name LIKE '___hi';

--Selects all elements with a name that ends with hi and has at least 3 characters before it
SELECT *
FROM table
WHERE name LIKE '%___hi';
```
