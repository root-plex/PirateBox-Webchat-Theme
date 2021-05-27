# PirateBox-Webchat-Theme
PirateBox Webchat Theme
First download  this repository. got to sftp://root@192.168.77.1 and backup/delete the files on /opt/piratebox/www/content and /opt/piratebox/www_content
extract the zip files to /opt/piratebox/www/content and /opt/piratebox/www_content make sure you have php enable.

Activate PHP
This mod requires PirateBox 1.1. 

PHP should be ready to run. To activate PHP on PirateBox, you need to edit /opt/piratebox/conf/lighttpd/lighttpd.conf and remove the # in front of the last line: #include “/opt/piratebox/conf/lighttpd/fastcgi-php.conf”

The can be achieved with the following command, too:

[root@piratebox~]$
sed -i -e 's|^#include "/opt/piratebox/conf/lighttpd/fastcgi-php.conf"|include "/opt/piratebox/conf/lighttpd/fastcgi-php.conf"|' \ 

/opt/piratebox/conf/lighttpd/lighttpd.conf


After this make a reboot. All .php files are processed, as long as these are placed in the /content/
