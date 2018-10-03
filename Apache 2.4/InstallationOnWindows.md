# APACHE 2.4 Code tips

## Windows installation

If you are installing a local server at work I would recommend installing Apache, PHP and MySQL separately as WAMP server requires Admin Privileges

### Download

[Apache lounge: http://www.apachelounge.com/download/](http://www.apachelounge.com/download/)

### Before installing

Check that you have installed C++ Redistributables listed

### STEPS

1. unzip or extract and rename the directory to Apache

2. Go to apache/conf and open httpd.conf

3. Search for all references to Apache24 and rename then to apache or location of apache file C:/webserver/apache

4. Start the server by going to commanfd prompt and locating c:\weberver\apache\bin

5. Then execute httpd (just type httpd in the prompt).

Run apache 2.4 as a windows service - ONLY do this if you have Admin rights

1. in command prompt cd to the bin folder

2. > httpd -k install

3. Start service from command line >net start apache2.4

4. To Stop service from command line >net stop apache2.4

5. To remove service > httpd -k uninstall

6.  You can also stop and start the servioce using windows services
