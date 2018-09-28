### PHPUnit Test Code Tips

## Specifically for Moodle

### In your config.php file

Add the following:

```php
$CFG->phpunit_prefix = 'phpu_';
$CFG->phpunit_dataroot = 'location\\phpu_sitedata';

$CFG->phpunit_dbtype    = 'mysqli';      // 'pgsql', 'mariadb', 'mysqli', 'mssql', 'sqlsrv' or 'oci'
$CFG->phpunit_dblibrary = 'native';     // 'native' only at the moment
$CFG->phpunit_dbhost    = 'localhost';  // eg 'localhost' or 'db.isp.com' or IP
$CFG->phpunit_dbname    = 'databasename';     // database name, eg moodle
$CFG->phpunit_dbuser    = 'root';   // your database username
$CFG->phpunit_dbpass    = 'XXXXXX';   // your database password
```

in CLI

```php
php site\admin\tool\phpunit\cli\init.php
```

If your work is using Windows make sure the environment variable is set for your PHP location.  C:\php\php5.6
No slash at the end of 5.6.