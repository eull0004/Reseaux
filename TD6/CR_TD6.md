# COMPTE RENDU

## Travail à réaliser : installation d’un serveur ftp

### 1. Mettre à jour le système : sudo apt update puis sudo apt upgrade.
![](TD6/TD6/img_1_1.png)

### 2. Installation paquet openssh-server pour pouvoir se connecter à distance à la machine.
![](TD6/TD6/img_1.2.png)

### 3. Installer maintenant le paquet vsftpd en utilisant l’outil apt.
![](TD6/TD6/img_1.3.png)

### 4. Utiliser la commande sudo nano /etc/vsftpd.conf pour éditer la configuration du serveur :
### a) Régler la configuration pour activer seulement IPv4.
![](TD6/TD6/img_1.4a.png)

### b) Autoriser les connexions anonymes.

### c) Ajouter une bannière d’accueil personnalisée à votre serveur.

![](TD6/TD6/img_1.4c.png)

### 5. Tenter de parcourir l’arborescence.
![](TD6/TD6/img_1.5 .png)

### 6.
### a) Modifier la configuration pour activer la ligne chroot_local_user=YES
![](TD6/TD6/img_1.6.png)

### b) Tester la connexion avec l’utilisateur iut : que constate-ton ?
![](TD6/TD6/img_1.6b.png)

### c)  Résoudre le problème en créant un répertoire Documents dans /home/iut puis en retirant les droits en écriture de l’utilisateur iut sur son $HOME.
![](TD6/TD6/img_1.6c.png)

### d) Vérifier le bon fonctionnement.
![](TD6/TD6/img_1.6d.png)