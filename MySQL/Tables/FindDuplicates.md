### MySQL Code Tips

## Find duplicates from a table;

```mysql
SELECT name, COUNT(*) c FROM table GROUP BY name HAVING c > 1;
```