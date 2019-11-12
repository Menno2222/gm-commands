# Instructions on how to install Ether Saga Odyssey server
Note these instructions are extremely rough and pulled from a variety of sources to try and make a single complete guide.
## Environment
 - Ubuntu Server 12
 - winscp
 - putty(if you are using a remote server)
 - openssh-server
 - mysql-server
 - apache2
 - php5 php5-mysql php-auth php5-xmlrpc libapache2-mod-php5 php5-mcrypt
 - phpmyadmin

## Setup
1. The first step is to install your operating system and define a root password using ``sudo passwd`` Once this password is defined you can reboot the system and login with username ``root`` and the password you set.
2. Next you need to run a few commands to install some prerequisites. 
```
apt-get update
apt-get install openssh-server
apt-get install mysql-server
apt-get install apache2
apt-get install php5 php5-mysql php-auth php5-xmlrpc libapache2-mod-php5 php5-mcrypt
apt-get install phpmyadmin
```
   As these are installing you will be asked to set passwords. Make your passwords strong. It will ask you if you are using/want to install apache2 or lighttpd, choose apache2. Everything else is fairly self explanatory i.e. if it asks what your mysql password is type in your mysql password.
   
3. Once all of this is done you need your servers ip, you get this by running ``ifconfig`` Once you have this ip open a web browser on another machine and navigate to ``yourserverip/phpmyadmin`` Login to phpmyadmin using the password you created in step 2. 

4. Make a new database called ``kdxy`` and import ``kdxy2.sql``

5. Open winscp and connect to a new site using SFTP. 
 - The ``Host Name`` will be your servers ip
 - The ``Port Number`` is ``22``
 - The ``username`` is ``root`` 
 - The ``password`` is the password you set in step 2.
6. Copy the contents of ``kdxy.zip`` to the ``root`` folder and set RWX permissions recursively. As well as copy over the extra libs required for a linux install.
7. Sync up the client and server by copying ``kdxy/gamed/config/gshop.data`` and ``kdxy/gamed/config/gshopsev.data`` from the server to the client. Copy ``elements.data`` from the client to the server.
8. Change the first four ips in ``/root/kdxy/glinkd/ gamesys.conf `` and change 1 ip in ``/var/www/includes/config.php`` to match your servers and ip. As well as edit ``table.xml`` to match your mysql root passwords.
9. In the client navigate to ``element/userdata/server/serverlist.txt`` and change the ip to your servers ip.
10. To start the server login as root, make sure you are in the root directory and run ``./start``
11. Create a registration page and place it in ``var/www``
