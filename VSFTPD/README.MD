## I- Installation:
### 1- login en tant que super utilisateur
### 2- sudo apt update -y
### 3- sudo apt install vsftpd -y
### 4- sudo vsftpd -v
### 5- sudo systemctl status vsftpd
### 6- ip addr

## II-Ajouter nouvel utilisateur:
### 1- sudo adduser ftpuser
### 2- sudo mkdir /home/ftpuser/ftp
### 3- sudo mkdir /home/ftpuser/ftp/fichier
### 4- chown nobody:nogroup /home/ftpuser/ftp
### 5- chmod a-w /home/ftpuser/ftp
### 6- chown ftpuser:ftpuser /home/ftpuser/ftp/fichier

## II- Configuration:
### 1- sudo cp /etc/vsftpd.conf /etc/vsftpd.conf.bak
### 2- http://vsftpd.beasts.org/vsftpd_conf.html
### sudo nano /etc/vsftpd.conf

## III- Test final
### sudo systemctl status vsftpd