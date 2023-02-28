
# PARTIE 1: *Les données ICMP locales*
## 1. **Identifier les adresses d'interface de votre ordinateur**

### a) **Noter l'adresse IP (notée inet avec ifconfig) et l'adresse physique (MAC, notée ether) de l'interface de votre ordinateur.**
_adresse IP :_ 10.31.4.58

_adresse MAC :_ 5C-60-BA-C6-6E-37 

![](img/TD2/img1aDONE.png)

### b) **Demandez à un binôme voisin de fournir l'adresse IP de son ordinateur et donnez-lui la votre. Ne lui fournissez pas votre adresse MAC pour le moment.**

_adresse IP du voisin :_ 10.31.4.59

![](img/TD2/img1bVoisinDONE.png)

## 2. **Commencer à capturer des données avec Wireshark**

### a) **Sélectionner l’interface correspondant au réseau local.**

![](img/TD2/img2a.png)

### b) **Cliquer sur l’aileron de requin pour démarrer la capture ! Les lignes de données s'affichent en différentes couleurs selon le protocole :**

![](img/TD2/img2b.png)

### c) **Pour cet atelier, il suffit de limiter l’affichage aux données ICMP (correspondant au ping) :**

![](img/TD2/img2c.png)

### c) et e) **Afficher la fenêtre d'invite de commandes ouverte précédemment et envoyer une requête ping à l'adresse IP du voisin :** et **Arrêter la capture en cliquant sur le gros carré rouge … **

![](img/TD2/img2d.png)
![](img/TD2/img2e.png)

## 3.
### a) **Cliquer sur la première trame de requête ICMP dans la partie supérieure de Wireshark.**
_L'adresse IP Source correspond à notre machine et l'adresse IP destination à la machine voisine._

![](img/TD2/img3a.png)

### b) **Afficher les adresses MAC de la destination et de la source.**

![](img/TD2/img3b.png)

### c) **L'adresse MAC de la source correspond-elle à l'interface de votre ordinateur ?**
_OUI, Les adresses correspondent bien_

### d) **L'adresse MAC de la destination correspond-elle à celle de l'ordinateur de votre voisin ?**
_OUI, Les adresses correspondent bien_

### e) **Comment votre ordinateur obtient-il l'adresse MAC de l'ordinateur destinataire des requêtes ping ?**
_grâce a l'ARP(adress Resolution protocol) qui permet de récupérer l'addresse MAC d'un autre appareil se trouvant sur le meme réseau IPv4._

# Partie II : Les données ICMP distantes
## 1. **Nouvelle capture**

### b) **Le processus de capture étant actif, envoyez une requête ping aux trois URL de sites web suivantes : www.yahoo.com; www.cisco.com; www.google.com**
_YAHOO :_ 
![](img/TD2/img1bPINGyahoo_PartII.png)

![](img/TD2/img1b_PartII(yahoo).png)

_CISCO :_ 
![](img/TD2/img2bPINGcisco_PartII.png)

![](img/TD2/img1b_PartII(cisco).png)

_GOOGLE :_
![](img/TD2/img2bPINGgoogle_PartII.png)

![](img/TD2/img1b_PartII(google).png)

## 2. **Examen et analyse des données des hôtes distants**
### b) **Indiquer les adresses IP et MAC de destination pour les trois sites :**
_YAHOO :_ 

*IP :* 87.248.100.216          
*MAC :* 68:05:ca:00:cd:7e

_CISCO :_

*IP :* 23.217.184.159          
*MAC :* 68:05:ca:00:cd:7e

_GOOGLE :_ 

*IP :* 142.250.75.228        
*MAC :* 68:05:ca:00:cd:7e

### c) **Qu'y a-t-il d'important à retenir de ces informations ? En quoi ces informationsdiffèrent-elles des informations de requêtes ping locales reçues dans la partie I ? **
 _Déjà l'adresse MAC est identique pour les trois sites destinataires des pings. Ensuite, contrairement à la première partie l'adresse IP des 3 sites sont diamétralement différentes indiquant que les machines ne sont pas du tout proches malgré que l'adresse MAC ne diffèrent pas._