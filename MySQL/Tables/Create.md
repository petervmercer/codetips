### MySQL Code Tips

## Create Table

```mysql
CREATE TABLE IF NOT EXISTS tablename (
`id` bigint(10) NOT NULL AUTO_INCREMENT,
`firstname` varchar(100) NOT NULL,
`lastname` varchar(100) NOT NULL,
`email` varchar(100) NOT NULL,
`postcode` varchar(4) NOT NULL DEFAULT '',
`uuid` varchar(50) NOT NULL,
PRIMARY KEY (`id`),
UNIQUE KEY `mdl_tablename_uix` (`email`,`uuid`),
KEY `mdl_tablename_email_ix` (`email`),
KEY `mdl_tablename_uuid_ix` (`uuid`)
)ENGINE=InnoDB  DEFAULT CHARSET=utf8 COLLATE=utf8_bin COMMENT='One record for each person';
```