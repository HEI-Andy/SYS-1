Installation:
-> sudo apt update -y
-> sudo apt install vsftpd -y
-> sudo vsftpd -v
-> sudo systemctl status vsftpd
-> ip addr

Ajouter nouvel utilisateur:
-> sudo adduser ftpuser
-> sudo mkdir /home/ftpuser/ftp
-> sudo mkdir /home/ftpuser/ftp/fichier
-> chown nobody:nogroup /home/ftpuser/ftp
-> chmod a-w /home/ftpuser/ftp
-> chown ftpuser:ftpuser /home/ftpuser/ftp/fichier

Configuration:
-> sudo cp /etc/vsftpd.conf /etc/vsftpd.conf.bak
-> http://vsftpd.beasts.org/vsftpd_conf.html
->sudo nano /etc/vsftpd.conf

Test final
-> sudo systemctl status vsftpd