Installation:
-> log_in en tant que super utilisateur
-> Telechargement de apache:  apt-get install apache2
-> verification si apache est bien installé: /etc/init.d/apache2 status

Configuration :
-> editer apache pour qu'il peut se connecter a notre site: nano /etc/apache2/apache2.conf   (version 2 de apache)
-> trouver var/www   et le remplacer avec notre dossier www
-> une autre configuration du root: sudo nano /etc/apache2/sites-enabled/000-default.conf  (pour virtual host, VMWARE)
-> re-démarré le serveur: /etc/init.d/apache2 restart