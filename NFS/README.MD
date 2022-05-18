## I- Installation:
### 1- se connecter an tant que supar utilisateur
### 2- apt-get install nfs-kernel-server

## II-Configuration:
### créer un fichier de partage: cd/ect/exports/

### configuration des adresses IP dans /home/nfs
### nano/etc/exports/
### configurer l'adresse client du serveur sur l'adresse IP server:
### /home/nfs     198.165.10/24(rw,async,no_root_squash)

## III- Redémarer nfs-server:
### /etc exports/ service nfs-kernel-server restart
## IV- récupérer l'IP serveur pour le connecter sur le machine client:
### ip addr

## V- Vérification connexion nfs:
### showmount -e 198.165.0.250