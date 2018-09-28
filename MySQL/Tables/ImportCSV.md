### MySQL Code Tips

## Import CSV;

This is not properly tested but a good starting point if you have to do this via command line

```mysql
LOAD DATA LOCAL INFILE '/filelocation/filename.csv'
INTO TABLE tablename
FIELDS TERMINATED BY ','
    ENCLOSED BY '"'
LINES TERMINATED BY '\n'
IGNORE 1 LINES
(first,last,email,uuid)
```