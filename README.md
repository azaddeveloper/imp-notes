# imp-note

**Url for make zip in putty or terminal**
   Main url:https://www.howtogeek.com/248780/how-to-compress-and-extract-files-using-the-tar-command-on-linux/

sudo tar -czvf where to download(/var/abc.tar.gz) folder path for(/var/www/abc)

ex->  tar -czvf /data/web/e18943/html/backup-20-08-201.tar.gz /data/web/e18943/html

with exclude command use for left that floder 
sudo tar -czvf where to download(/var/abc.tar.gz) folder path for(/var/www/abc) --exclude=/var/www/abc/xyz


Copy in putty 
sudo cp /path/to/source /path/to/dest/directory/
ex 
sudo cp -r /var/www/html/pressureproweb/ppnew/* /var/www/html/

copy hidden file
cp -r /etc/skel/. /home/<new_user>  // add . in place of *
show hidden file 
ls -ld .?* 



unzip in putty

sudo path to the file
i)chnge direcory 
tar -xvzf /home/lifedata/backup-29-08-201.tar.gz

permission 
 sudo chmod 777 /home/lifedata/public_html/devlop

sudo chmod 777 -R /var/www/html/develop

delete in putty 
sudo rm -rf /folder


Pastbin for share code to other one


Angular Imp URLs:
https://github.com/manavpandya?tab=repositories



vs code ext install esbenp.prettier-vscode




update php.ini
1.sudo nano  /etc/php.ini
2.
--------------
upload_max_filesize=64M
post_max_size=64M
max_execution_time=100
--------------
3.save by ctr+o then enter ctr+x
4.sudo /etc/init.d/httpd restart

save git password in terminal
1.git config --global credential.helper store 
then type once username and password it will save for 15 min
to increase timeout 
# Set the cache to timeout after 1 hour (setting is in seconds)
git config --global credential.helper 'cache --timeout=3600'


// merge multple files into one file
cat *.sql  > .all_files.sql

import db in ubuntu
1. Go in directory
   cd /opt/lampp/bin
2. ./mysql -h localhost -u root -p  <  ; // /mysql -h localhost -u root -p db_name < sql_file_path ;
