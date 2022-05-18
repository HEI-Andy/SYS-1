## I- Installation:
### 1- login en tant que super utilisateur
### 2- apt get install samba

## II- Ajoutér un compte utilisateur à la base de données Samba
### 1- sudo smbpasswd -a NOM UTILISATEUR (MOT DE PASSE)
### 2- sudo service smbd reload

## III- Configurer le partage de données
### 1- gedit /etc/samba/smb.conf