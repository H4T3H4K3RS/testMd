

**Solution:**

The SQL query to join the SUBS and CITY tables is as follows: 

```sql
SELECT SUBS_ID, NAME, CITY.NAME, BEG_DT, END_DT
FROM SUBS
INNER JOIN CITY
ON SUBS.CITY_ID = CITY.CITY_ID
```

The result of the joining SUBS and CITY tables is shown in the table below:

| SUBS_ID | NAME | CITY.NAME | BEG_DT      | END_DT       |
|---------|------|-----------|-------------|--------------|
| 2       | Vasya| Omskgrad  | 1900-01-01  | 2001-01-01   |
| 2       | Petya| Omsk      | 2001-01-01  | 2010-01-01   |
| 2       | Petya| Tomsk     | 2010-01-01  | 9999-01-01   |