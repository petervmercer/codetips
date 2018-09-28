### MySQL Code Tips

## Describe table;

```mysql
DESCRIBE tablename;
```

Example below of the output using a Totara 9 DB user table


```text
mysql> DESCRIBE mdl_user;

+-------------------+--------------+------+-----+-----------+----------------+
| Field             | Type         | Null | Key | Default   | Extra          |
+-------------------+--------------+------+-----+-----------+----------------+
| id                | bigint(10)   | NO   | PRI | NULL      | auto_increment |
| auth              | varchar(20)  | NO   | MUL | manual    |                |
| confirmed         | tinyint(1)   | NO   | MUL | 0         |                |
| policyagreed      | tinyint(1)   | NO   |     | 0         |                |
| deleted           | tinyint(1)   | NO   | MUL | 0         |                |
| suspended         | tinyint(1)   | NO   |     | 0         |                |
| mnethostid        | bigint(10)   | NO   | MUL | 0         |                |
| username          | varchar(100) | NO   |     |           |                |
| password          | varchar(255) | NO   |     |           |                |
| idnumber          | varchar(255) | NO   | MUL |           |                |
| firstname         | varchar(100) | NO   | MUL |           |                |
| lastname          | varchar(100) | NO   | MUL |           |                |
| email             | varchar(100) | NO   | MUL |           |                |
| emailstop         | tinyint(1)   | NO   |     | 0         |                |
| icq               | varchar(15)  | NO   |     |           |                |
| skype             | varchar(50)  | NO   |     |           |                |
| yahoo             | varchar(50)  | NO   |     |           |                |
| aim               | varchar(50)  | NO   |     |           |                |
| msn               | varchar(50)  | NO   |     |           |                |
| phone1            | varchar(20)  | NO   |     |           |                |
| phone2            | varchar(20)  | NO   |     |           |                |
| institution       | varchar(255) | NO   |     |           |                |
| department        | varchar(255) | NO   |     |           |                |
| address           | varchar(255) | NO   |     |           |                |
| city              | varchar(120) | NO   | MUL |           |                |
| country           | varchar(2)   | NO   | MUL |           |                |
| lang              | varchar(30)  | NO   |     | en        |                |
| calendartype      | varchar(30)  | NO   |     | gregorian |                |
| theme             | varchar(50)  | NO   |     |           |                |
| timezone          | varchar(100) | NO   |     | 99        |                |
| firstaccess       | bigint(10)   | NO   |     | 0         |                |
| lastaccess        | bigint(10)   | NO   | MUL | 0         |                |
| lastlogin         | bigint(10)   | NO   |     | 0         |                |
| currentlogin      | bigint(10)   | NO   |     | 0         |                |
| lastip            | varchar(45)  | NO   |     |           |                |
| secret            | varchar(15)  | NO   |     |           |                |
| picture           | bigint(10)   | NO   |     | 0         |                |
| url               | varchar(255) | NO   |     |           |                |
| description       | longtext     | YES  |     | NULL      |                |
| descriptionformat | tinyint(2)   | NO   |     | 1         |                |
| mailformat        | tinyint(1)   | NO   |     | 1         |                |
| maildigest        | tinyint(1)   | NO   |     | 0         |                |
| maildisplay       | tinyint(2)   | NO   |     | 2         |                |
| autosubscribe     | tinyint(1)   | NO   |     | 1         |                |
| trackforums       | tinyint(1)   | NO   |     | 0         |                |
| timecreated       | bigint(10)   | NO   |     | 0         |                |
| timemodified      | bigint(10)   | NO   |     | 0         |                |
| trustbitmask      | bigint(10)   | NO   |     | 0         |                |
| imagealt          | varchar(255) | YES  |     | NULL      |                |
| lastnamephonetic  | varchar(255) | YES  | MUL | NULL      |                |
| firstnamephonetic | varchar(255) | YES  | MUL | NULL      |                |
| middlename        | varchar(255) | YES  | MUL | NULL      |                |
| alternatename     | varchar(255) | YES  | MUL | NULL      |                |
| totarasync        | tinyint(1)   | NO   | MUL | 0         |                |
+-------------------+--------------+------+-----+-----------+----------------+
54 rows in set (0.03 sec)

```

