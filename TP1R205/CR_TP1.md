# Partie 3
## La commande host (sous Linux)
### 2. Utilisez la commande host pour retrouver :
**adresse IP du site www.free.fr** : 

__l'addresse : 212.27.48.10__

![](TD1_R2.05/TD1/P3_host_Q2_1.png)

**le FQDN de 194.57.105.10** : 

__le FQDN : mediacenter-proxy.univ-reims.fr__

![](TP1R205/TP1R205/P3_host_Q2_2.PNG)

**les FQDN des serveurs dns de la zone google.com :** 

__par10s42-in-f14.1e100.net__
__mad01s26-in-f14.1e100.net__
__mad01s26-in-f174.1e100.net__

![](TP1R205/TP1R205/P3_host_Q2_3.PNG)

**les FQDN des serveurs de messagerie électronique de la zone google.com :**

__wm-in-f27.1e100.net__  
__wr-in-f26.1e100.net__  
__wr-in-f27.1e100.net__  
__wo-in-f26.1e100.net__  
__wm-in-f26.1e100.net__

![](TP1R205/TP1R205/P3_host_Q2_4.PNG)


### 4. Quelle commande permet de récupérer la liste des serveurs racines ?

__la commande dig NS : dig NS . www.google.fr__

### 5. Combien de serveurs gèrent la zone fr ?
__commande dig NS fr. www.google.fr : 4 serveurs__


## La commande nslookup (sous Windows)
### 2. Quelle est l'information produite par l'exécution de la commande ?
![](TP1R205/TP1R205/img1_PartWindows.png)

### 3. Quelle instruction doit-on inscrire pour récupérer l'adresse IP du serveur cleo.univ-reims.fr ?
![](TP1R205/TP1R205/img3_partWindows.png)

### 4. La réponse fait-elle autorité ? Expliquez !
__Elle ne fait pas autorité car le serveur cleo.univ-reims.fr n'est pas le serveur cleo.univ-reims.fr principal/par défaut.__

### 5. Quelle instruction permet de changer le serveur de nom à utiliser ?
![](TP1R205/TP1R205/img5_PartWindows.png)

### 6. Relancer la commande permettant de récupérer l'adresse IP du serveur cleo.univ-reims.fr
![](TP1R205/TP1R205/img6_PartWindows.png)


### 7. La réponse fait-elle autorité ? Expliquez !
__Oui, grâce à la commande précédente on a pu configuer ce serveur comme le principal donc lui donner autorité.__

### 8. Quelle instruction permet de changer le type de requête afin de récupérer les enregistrements de type serveurs de noms ?
![](TP1R205/TP1R205/img8_PartWindows.png)

### 9. Quels sont les FQDN et les adresses IP de la zone univ-reims.fr ?
![](TP1R205/TP1R205/img9_PartWindows.png)




## La commande dig

### 2. Quelle est l'utilisation de la commande dig permettant de récupérer les adresses IP des serveurs de messagerie électronique de la zone univ-reims.fr en utilisant le serveur de noms anne.univ-reims.fr ? 
__la commande  : dig MX univ-reims.fr @anne.univ-reims.fr__


### 3. Quelle requête permet de tracer le chemin de délégation depuis le serveur racine vers la cible www.univ-reims.fr ?
__la commande : dig +trace www.univ-reims.fr__