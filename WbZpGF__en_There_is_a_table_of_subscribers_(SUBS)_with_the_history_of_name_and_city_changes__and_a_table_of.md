

Answer:

**SQL Query:**

```sql
SELECT 
  s.SUBS_ID, s.NAME, s.BEG_DT, s.END_DT,
  c.CITY_ID, c.NAME, c.BEG_DT, c.END_DT
FROM SUBS s
  LEFT JOIN CITY c
    ON s.CITY_ID = c.CITY_ID
    AND s.BEG_DT < c.END_DT
    AND s.END_DT > c.BEG_DT;
```

**Result:**

| SUBS_ID | NAME  | BEG_DT   | END_DT   | CITY_ID | NAME      | BEG_DT   | END_DT   |
| ------- | ----- | -------- | -------- | ------- | --------- | -------- | -------- |
| 2       | Vasya | 1900-01-01 | 2001-01-01 | 4      | Omsk      | 1990-01-01 | 9999-01-01 |
| 2       | Petya | 2001-01-01 | 2010-01-01 | 4      | Omsk      | 1990-01-01 | 9999-01-01 |
| 2       | Petya | 2010-01-01 | 9999-01-01 | 5      | Tomsk     | 1900-01-01 | 9999-01-01 |