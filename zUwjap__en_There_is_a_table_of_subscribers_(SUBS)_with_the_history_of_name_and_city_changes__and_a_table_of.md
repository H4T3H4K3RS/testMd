

**Solution:** 

SQL Query:
```sql
SELECT SUBS.SUBS_ID, SUBS.NAME, SUBS.BEG_DT, SUBS.END_DT, CITY.NAME 
FROM SUBS
INNER JOIN CITY
ON SUBS.CITY_ID = CITY.CITY_ID
```

Result Table:

| SUBS_ID | NAME   | BEG_DT      | END_DT      | NAME    |
|---------|--------|-------------|-------------|---------|
| 2       | Vasya  | 1900-01-01  | 2001-01-01  | Omskgrad|
| 2       | Petya  | 2001-01-01  | 2010-01-01  | Omsk    |
| 2       | Petya  | 2010-01-01  | 9999-01-01  | Tomsk   |