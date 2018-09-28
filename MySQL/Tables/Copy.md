### MySQL Code Tips

## Copy table

** Not used or tested at this point

```mysql
CREATE TABLE newtable LIKE oldtable; 
INSERT newtable SELECT * FROM oldtable;
```
