# fix-wordpress-permissions.sh

A script to configure WordPress file permissions based on recommendations from http://codex.wordpress.org/Hardening_WordPress#File_permissions


Typically, all files should be owned by your user (ftp) account on your web server, and should be writable by that account. On shared hosts, files should never be owned by the webserver process itself (sometimes this is www, or apache, or nobody user).

You need to upload the .sh file, where your website or wordpress is being hosted i.e. the directory/path/wordpress for eg. /home/admin/web/mywebsite/public_html


## usage:
1. You need to upload the .sh file over here using filezilla or scp or cybercuk or whatever software you want to use.
2. In your wordpress directory execute  sudo sh ./fix-wordpress-permissions.sh /home/admin/web/yourwebsite-goes-here/public_html 

NB. Please do note that this is my directory and your directory can be different. you need to be in the directory of your wordpress installation to execute the command.

3. After that wait some time it should work