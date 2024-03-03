download file di github.com/fendyzhang 8 8 

nano /etc/network/interfaces 

auto enpos3 

iface enpos3 inet static 

address 192.168.100.101/25 

gateway 192.168.100.1


nano /etc/resolv.conf 

nameserver 8.8.8.8 

nameserver 8.8.4.4

service networking restart

ip addr 

nano /etc/apt/sources.list

deb http://deb.debian.org/debian/ bullseye main contrib non-free 

apt update 

apt install apache2 -y

apt install php php-mysqli php-xml -y 

apt install mariadb-server -y 

mysql_secure_installation 
n
y 
123
123
y
y
y 
y

apt install phpmyadmin –y (192.168.100.101/php)

apt install proftpd –y

nano /etc/proftpd/proftpd.conf 

defaultroot /varr/www/html

service proftpd restart

chmod 777 /var/www/html (buka file zila)
-------------------------------------------------------
database name: db_jason
username: root
pass: 123
