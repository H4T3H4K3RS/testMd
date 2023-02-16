

**Solution:**

SQL query for joining SUBS and CITY tables:
```
SELECT s.SUBS_ID, s.NAME, c.NAME, s.BEG_DT, s.END_DT
FROM SUBS s
JOIN CITY c
ON s.CITY_ID = c.CITY_ID
```

Result table:

| SUBS_ID | NAME | CITY_NAME | BEG_DT | END_DT | 
|---------|------|-----------|--------|--------| 
|    2    | Vasya |  Omskgrad | 1900-01-01 | 2001-01-01 | 
|    2    | Petya |     Omsk  | 2001-01-01 | 2010-01-01 | 
|    2    | Petya |    Tomsk  | 2010-01-01 | 9999-01-01 |