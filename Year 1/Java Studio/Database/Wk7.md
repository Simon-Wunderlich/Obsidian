Created: May 14 2025
Class: [[Database]] 
- - -
## Part A

```sql
Q. 1
SELECT * FROM MOVIE;

Q. 2
SELECT MVTITLE FROM MOVIE;

Q. 3
SELECT COUNT(\*) FROM MOVIE;

Q. 4
SELECT *
FROM MOVIE
WHERE LOWER(MVTYPE) == 'horror';

Q. 5
SELECT *
FROM MOVIE
WHERE LOWER(MVTYPE) == 'horror' 
	AND NOMS > 0;

Q. 6
SELECT *
FROM MOVIE
WHERE (LOWER(MVTYPE) == 'horror' 
	AND NOMS > 0) 
	OR LOWER(MVTYPE) == 'comedy';

Q. 7
SELECT *
FROM MOVIE
WHERE (LOWER(MVTYPE) == 'horror' 
	AND NOMS > 0) 
	OR (LOWER(MVTYPE) == 'comedy' 
	AND NOMS > 0);

Q. 8
SELECT *
FROM MOVIE
WHERE AWRD > 3;

Q. 9
SELECT *
FROM MOVIE
WHERE MVTITLE LIKE '%Nuremberg%';
```

## Part B

```sql
Q. 10
SELECT AVG(NUMRENT)
FROM MEMBER;

Q. 11
SELECT MMBNUMB, JOINDATE
FROM MEMBER;

Q. 12
SELECT MMBNUMB, STRFTIME('%d/%m/%Y', JOINDATE) AS "JOINDATE"
FROM MEMBER;

Q. 13 
SELECT MMBNAME, 
STRFTIME('%d/%m/%Y', JOINDATE) AS "JOINDATE", 
ROUND(julianday('now') - julianday(JOINDATE)) AS "timeDiffDays", 
ROUND((julianday('now') - julianday(JOINDATE))/365.25) AS "timeDiffYears"
FROM MEMBER;

Q. 14
SELECT MMBNAME, 
STRFTIME('%d/%m/%Y', JOINDATE) AS "JOINDATE", 
ROUND(julianday('now') - julianday(JOINDATE)) AS "timeDiffDays", 
ROUND((julianday('now') - julianday(JOINDATE))/365.25) AS "timeDiffYears"
FROM MEMBER
ORDER BY MMBNAME ASC;

Q. 15
SELECT MMBNAME, 
STRFTIME('%d/%m/%Y', JOINDATE) AS "JOINDATE", 
ROUND(julianday('now') - julianday(JOINDATE)) AS "Number of days since joined", 
ROUND((julianday('now') - julianday(JOINDATE))/365.25) AS "Number of years since joined"
FROM MEMBER
ORDER BY timeDiffDays DESC;

Q. 16
SELECT MMBNAME AS  "Member name", 
STRFTIME('%d/%m/%Y', JOINDATE) AS "Date joined", 
ROUND(julianday('now') - julianday(JOINDATE)) AS "timeDiffDays", 
ROUND((julianday('now') - julianday(JOINDATE))/365.25) AS "timeDiffYears"
FROM MEMBER
ORDER BY timeDiffDays DESC;
```