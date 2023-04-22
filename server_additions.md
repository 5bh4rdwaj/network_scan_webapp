# In the machine where website is to be hosted
* install php, nmap, apache2
* allow ufw firewall access to apache2 (80/tcp, 443/tcp)
* permit the usage of /var/www/html folder

add the following to the end of the command 'sudo crontab -e':
'*/30 * * * * nmap 192.168.29.1/24 -oN /var/www/html/nmap_output.html'