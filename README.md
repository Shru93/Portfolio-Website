# Portfolio-Website
Portfolio Website Test for Resume (Instructions Below)

Deploy Web application on AWS Cloud using EC2 Instance

1. Create EC2 Instance
2. Connect with EC2 Instance Connect
3. Login as a root user $sudo su 
4. yum update -y
5. yum install httpd
6. systemctl status httpd
7. make one directory for files (mkdir [name of directory])
8. connect to GitHub with HTTP link into GitHub wget https://github.com/shridharDesai/Portfolio-Website.git
9 Let’s see list of downloaded from GitHub to Folder “[name of dir]” ls -l
10.Download main.zip folder and unzip (zip folder link get from zip into )
wget  https://github.com/shridharDesai/Portfolio-Website/archive/refs/heads/main.zip
11. ls -l
total 876
-rw-r--r--. 1 root root 274010 Jul 31 13:20 Portfolio-Website.git
-rw-r--r--. 1 root root 619358 Jul 31 13:26 main.zip
12. Unzip main.zip
Change directory to executable file
13. ls -l
total 876
drwxr-xr-x. 5 root root     77 Jul 31 12:27 Portfolio-Website-main
-rw-r--r--. 1 root root 274010 Jul 31 13:20 Portfolio-Website.git
-rw-r--r--. 1 root root 619358 Jul 31 13:26 main.zip
14. cd Portfolio-Website-main
-rw-r--r--. 1 root root   178 Jul 31 12:27 README.md
drwxr-xr-x. 3 root root    94 Jul 31 12:27 css
-rw-r--r--. 1 root root 10600 Jul 31 12:27 index.html
drwxr-xr-x. 2 root root    23 Jul 31 12:27 js
drwxr-xr-x. 6 root root   154 Jul 31 12:27 plugins
15. To enter into html folder where actual webpage available-
mv * /var/www/html/
16. Change directory to html
cd  /var/www/html
17. l s -l
-rw-r--r--. 1 root root   178 Jul 31 12:27 README.md
drwxr-xr-x. 3 root root    94 Jul 31 12:27 css
-rw-r--r--. 1 root root 10600 Jul 31 12:27 index.html
drwxr-xr-x. 2 root root    23 Jul 31 12:27 js
drwxr-xr-x. 6 root root   154 Jul 31 12:27 plugins
17. Go to Instance – Security Group – Inbound Rules – Edit Inbound Rules (save)
HTTP -  (80) - Anywhere IPv4
HTTPS – (443) - Anywhere IPv4
18. systemctl status httpd
-provides a means to check the status of any systemd service running on dedicated server hosting
19. systemctl enable httpd
-Enable a service, without starting it.
20. Creating link -
Created symlink /etc/systemd/system/multi-user.target.wants/httpd.service → /usr/lib/systemd/system/httpd.service.
21. Start Link –
Systemctl start httpd
is the command-line tool that manages the systemd system and service manager in Linux. It lets users control and manage system services and units with commands to start, stop, restart, and check their status.
22. Copy – Auto-assigned elastic IP into browser
Web application Deployed and Open.

//if you see 'It works!' on the website - make sure to rename your .html file to index.html and make sure it is in /var/www/html. If you see any other errors, ensure to go through the steps again to avoid any mistakes, even the slightest of typos can mess it up :)//


*****These are not my development instructions above - I have followed this tutorial https://github.com/shridharDesai/Portfolio-Website/archive/refs/heads/main.zip to learn and set this up, however index.html on my page is configured by me*****


