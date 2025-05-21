Created: May 21 2025
Class: [[JOIN]] 
- - -
### Part A
``` sql
Q. 1
SELECT m.MVTITLE AS Title, d.DIRNAME AS Director
FROM MOVIE as m
JOIN DIRECTOR AS d ON m.DIRNUMB = d.DIRNUMB;

Q. 2
SELECT m.MVTITLE AS Title, d.DIRNAME AS Director
FROM MOVIE as m
NATURAL JOIN DIRECTOR as d;

```
