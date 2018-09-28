### MySQL Code Tips

## Alter Table

### Table Name

```mysql
ALTER TABLE old_table RENAME new_table;
```
OR
```mysql
RENAME TABLE old_table TO new_table;
```

RENAME TABLE, unlike ALTER TABLE, can rename multiple tables within a single statement: 

```mysql
RENAME TABLE old_table1 TO new_table1,
             old_table2 TO new_table2,
             old_table3 TO new_table3;
```