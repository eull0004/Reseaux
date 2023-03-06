# COMPTE RENDU
# PARTIE 1: *Gestion d'un réseau dans fil - les trames "beacon"*
### **b) Observer la première trame et déterminer la gamme de fréquences et le canal utilisé.**
![]()
_La fréquence est de 2437 MHz donc c'est une bande ISM et son canal est le 6.

### **c) Quels sont les SSID des deux points d'accès qui émettent la plupart des trames de balises dans cette trace ?**
![]()

### **d) Quels sont les intervalles de temps entre les transmissions des trames de balises du point d'accès linksys_ses_24086 ? Du point d'accès du 30 Munroe Street ?**
![]()

### **e) Quelle est l'adresse MAC source de la trame beacon du 30 Munroe Street ?**
_00:16:b6:f7:1d:51_

### **f) Quelle est l'adresse MAC de destination de cette trame ?**
_ff:ff:ff:ff:ff:ff_

### **g) Les trames beacon de l’AP2 30 Munroe St avertissent que l’AP supporte 4 débits de base et 8 débits étendus. Quels sont ces débits ?**
![]()
![]()


# PARTIE 2: *Association/désassociation*
### **a) Quelles sont les deux trames émises par l’hôte juste après t = 49 pour clore l’association avec l’AP 30 Munroe St ?**
![]()

### **b) Combien de messages AUTHENTICATION sont envoyés du PC mobile vers l’AP linksys_ses_24086 (@MAC : Cisco_Li_f5:ba:bb) aux environs du temps t=49 ?**
![]()

### **c) L'hôte souhaite-t-il que l'authentification nécessite une clé ou soit ouverte ?**
![]()

### **d) L’AP linksys_ses_24086 émet-il une réponse AUTHENTICATION ?**
_Non_

### **e) L’hôte abandonne cette association et teste l’AP 30 Munroe St. À quels moments y a-t-il une trame AUTHENTICATION de l’hôte vers l’AP et quand y-a-t-il une réponse de l’AP ?**
![]()
_Il y a une trame authentification de l'hôte vers l'AP à t = 63. L'AP répond à t = 63._

### **f) À quel moment a-t-on une trame ASSOCIATION REQUEST de l’hôte vers l’AP 30 Munroe St et quand la réponse correspondante est-elle émise ?**
![]()
_On a une trame ASSOCIATION REQUEST de l'hôte vers l'AP à t = 63 et la réponse arrive un peu près toujours à t = 63_

### **g) Quels débits l’hôte peut-il utiliser ? L’AP ?**
_l'hôte:_
![]()
_l'AP:_
![]()

# PARTIE 3: *Transfert de données*
### **a) Trouver la trame 802.11 contenant le segment TCP SYN d’établissement de connexion de la première requête.**
![]()

### **b) Quels sont les trois adresses MAC dans la trame ? Laquelle de ces adresses est celle de l’hôte ? Du point d’accès ? De la passerelle ?**
_adresse MAC (hôte): 00:13:02:d1:b6:4f_  
_adresse MAC (point d'accès): 00:16:b6:f4:eb:a8_  
_adresse MAC (passerelle): 00:13:02:d1:b6:4f_

### **c)Quelle est l’adresse IP du terminal mobile ?**
 **Quelle est l’adresse IP de destination et à quelle interface correspond-t-elle ?**
 