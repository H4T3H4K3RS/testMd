

SQL Query:
```
SELECT 
  s.SUBS_ID, s.NAME, c.CITY_ID, c.NAME 
FROM 
  SUBS AS s 
  LEFT JOIN CITY AS c 
    ON s.CITY_ID = c.CITY_ID 
WHERE 
  s.BEG_DT <= CURRENT_DATE() AND 
  s.END_DT >= CURRENT_DATE()
```

Result of Joining SUBS and CITY Tables:

| SUBS_ID | NAME  | CITY_ID | NAME    |
|---------|-------|---------|---------|
| 2       | Petya | 5       | Tomsk   |