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

### DATETIME
Datetime is not a data type, stored as string or int

``` sql 
DATE(timeValue) --converts the date as text
TIME(timeValue) --converts the time as text
DATETIME(timeValue) --converts time and date to text
JULIANDAY(timeValue) --Days since noon in Greenwich on November 24, 4714 B.C.
UNIXEPOCH(timeValue) -- Days since unix epoch (1st Jan 1970)
STRFTIME('format', timeValue)
TIMEDIFF(timeValue, timeValue) --Returns string representing time difference
```
