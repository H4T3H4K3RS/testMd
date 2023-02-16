

**Solution:**

The SQL query to join the SUBS and CITY tables is as follows: 

```sql
SELECT 
    s.SUBS_ID, 
    s.NAME, 
    c.NAME,
    s.BEG_DT, 
    s.END_DT
FROM SUBS s
INNER JOIN CITY c ON s.CITY_ID = c.CITY_ID
WHERE 
    s.BEG_DT <= CURRENT_DATE
    AND s.END_DT >= CURRENT_DATE
    AND c.BEG_DT <= CURRENT_DATE
    AND c.END_DT >= CURRENT_DATE;
```

This query will return the following table:

| SUBS_ID | NAME  | NAME  | BEG_DT      | END_DT      |
|---------|-------|-------|-------------|-------------|
| 2       | Petya | Tomsk | 2010-01-01  | 9999-01-01  |

The result of joining these two tables shows that the name of the subscriber with `SUBS_ID` 2 is Petya and the city is Tomsk, with the validity of this data being from the beginning of 2010 to the present.