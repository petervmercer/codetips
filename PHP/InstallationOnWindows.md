# PHP Code Tips

## Installation

### Windows instructions

For Windows

Go to windows.php.net

Download thread safe version

extract to c:/webserver/php

locate the name of the apache dll file in the php directory php5apache2_4.dll

IN APACHE

1. locate conf/httpd.conf and open it

2. add text to the bottom - Change for different versions of apache
```text
LoadModule php5_module "C:/php/php5apache2_4.dll"
AddHandler application/x-httpd-php .php
# configure the path to php.ini
PHPIniDir "C:/php"
```

⋅3. For development copy and rename the php.ini-development

*Environment variable* in Windows:

Have the folder not php - No close at the end of the folder
c:\php\php5.6