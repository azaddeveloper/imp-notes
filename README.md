# Terminal command for the zip,copy/move and permission 
    
    1. Make zip or create archive
    
        sudo tar -czvf where to download(/var/abc.tar.gz) folder path for(/var/www/abc)
        
    2. Exclude command use for exclude a folder of file
    
        sudo tar -czvf where to download(/var/abc.tar.gz) folder path for(/var/www/abc) --exclude=/var/www/abc/xyz
     
    3. Copy or move by terminal  
    
         sudo cp /path/to/source /path/to/dest/directory/
         ex  sudo cp -r /var/www/html/folder/* /var/www/html/
         copy hidden file
         sudo cp -r /var/www/html/folder/* /var/www/html/  // add . in place of *
         
    4. Show hidden file
    
        ls -ld .?* 
        
    5. Unzip or extract by terminal
    
        sudo tar -xvzf /filepath/
        
    6. Permission of the file
    
        sudo chmod 777 -R /var/www/html/develop
        
    7. Delete a file or folder by terminal 
    
         sudo rm -rf /file or filder path/
         
    8. Merge multple files into one file
        
         cat *.sql  > .all_files.sql
    
    For more detail
   https://www.howtogeek.com/248780/how-to-compress-and-extract-files-using-the-tar-command-on-linux/


# Common Changes in php.ini file on AWS server

    1. Open file by below commmand
        sudo nano /etc/php.ini
    
    2. find and replace according your need
        --------------
        upload_max_filesize=64M
        post_max_size=64M
        max_execution_time=100
        --------------
        
    3. Save it by ctr+o then enter ctr+x
    
    4. Then resetart server
    
        sudo /etc/init.d/httpd restart

# Save git credentails in terminal
    
    1.git config --global credential.helper store 
    then type once username and password it will save for 15 min
    to increase timeout 
    # Set the cache to timeout after 1 hour (setting is in seconds)
    git config --global credential.helper 'cache --timeout=3600'     
    
# import db in ubuntu
    1. Go in directory
        cd /opt/lampp/bin
    2. ./mysql -h localhost -u root -p  <  ; // /mysql -h localhost -u root -p db_name < sql_file_path ;    
        
        
-----------------------------------------------------------------------------------------

Pastbin for share code to other one
    https://pastebin.com/

vs code ext install esbenp.prettier-vscode

Angular Imp URLs:
https://github.com/manavpandya?tab=repositories











