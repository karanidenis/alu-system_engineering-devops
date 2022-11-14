more knowledge on webservers and applying skills by writing bash scripts that publish websites on our server. 
#!/usr/bin/env bash
# script to install nginx

sudo apt-get -y update
sudo apt-get -y install nginx
sudo chown -R $USER:$USER /var/www/html
echo "Holberton School" > /var/www/html/index.html
sudo service nginx restart
