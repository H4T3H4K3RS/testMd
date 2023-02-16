

Solution:

**Current Records**

SUBS:

| SUBS_ID | NAME  | CITY_ID | BEG_DT   | END_DT   |
| ------- | ----- | ------- | -------- | -------- |
| 2       | Petya | 5       | 2010-01-01 | 9999-01-01 |

CITY:

| CITY_ID | NAME    | BEG_DT   | END_DT   |
| ------- | ------- | -------- | -------- |
| 4       | Omsk    | 1990-01-01 | 9999-01-01 |
| 5       | Tomsk   | 1900-01-01 | 9999-01-01 |

**Result of Joining SUBS and CITY Tables**

The following SQL query can be used to join the SUBS and CITY tables:

```sql
SELECT SUBS.SUBS_ID, SUBS.NAME, CITY.NAME, SUBS.BEG_DT, SUBS.END_DT
FROM SUBS
INNER JOIN CITY
ON SUBS.CITY_ID = CITY.CITY_ID;
```

The result of the query will be as follows:

| SUBS_ID | NAME  | NAME    | BEG_DT   | END_DT   |
| ------- | ----- | ------- | -------- | -------- |
| 2       | Petya | Tomsk   | 2010-01-01 | 9999-01-01 |