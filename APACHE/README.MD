## I- Installation:
### 1- login en tant que super utilisateur
### 2- Téléchargement de apache:  apt-get install apache2
### 3- vérification si apache est bien installé: /etc/init.d/apache2 status

## II- Configuration :
### 1- éditer apache pour qu'il peut se connecter a notre site: nano /etc/apache2/apache2.conf   (version 2 de apache)
### 2- trouver var/www   et le remplacer avec notre dossier www
### 3- une autre configuration du root: sudo nano /etc/apache2/sites-enabled/000-default.conf  (pour virtual host, VMWARE)
### 4- re-démarré le serveur: /etc/init.d/apache2 restart