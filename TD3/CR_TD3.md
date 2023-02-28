# COMPTE RENDU
# PARTIE 1: *Analyser de trames Ethernet
## 1. Affichage des ARP et ICMP
![](img/TD3/img_1_PartI.png)

## 2.Examiner la première requête ping dans Wireshark
### **a) Echo (ping) request**
![](img/TD3/img_2_PartI.png)

### **b) Quelle est l'adresse MAC de la carte réseau de l'ordinateur ?**
_5C-60-BA-C6-6E-37_

### **c) Quelle est l'adresse MAC du PC voisin?**
_a remplir_

### **d) Echo (ping) reply**
![](img/TD3/img_2.5_PartI.png)

### **e) Pourquoi l'ordinateur envoie-t-il une requête ARP avant d'envoyer la première requête ping ?**
_Pour pouvoir communiquer avec un autre hôte de sous-réseau différent sans avoir à faire de modification sur la configuration réseau des périphériques._

## 3. Etudier la table d'adresses MAC
### **a) Affichage tables d'adresses MAC:**
![](img/TD3/img_3_PartI.png)

### **b) Sans compter les adresses de multidiffusion ou de diffusion, combien de paires d'adresses IP vers MAC de périphériques ont été acquises par ARP ?**
_5_

### **c)Envoyer de nouvelles requêtes ping à d’autres voisins ou à des sites distants. Votre PC a-t-il ajouté des adresses MAC supplémentaires à la table ? Si oui lesquelles ?**
_Oui, il a ajouté les adresses MAC de type dynamiques ayant l'IP auquel l'envoie de pings était destiné._

# PARTIE 2: *les réseaux locaux virtuels*
## 1. Configuration du réseau
### **a) Réseau mis en place sur Packet Tracer selon les consignes :**
![](img/TD3/img_1a_PartII.png)

### **b) Les différents PC peuvent-ils communiquer entre eux?**
_Oui, comme on peut le voir ci-dessous avec un échange entre le PC1 et le PC2._

![](img/TD3/img_1d_PartII.png)


### c) **Après modification des masque IP en masque/25, les PC continuent-ils à communiquer ?**
_Oui, avec la même situation que précedemment._

![](img/TD3/img_1b_PartII.png)

### d) **Ces 2 sous-réseaux sont-ils différents.** 
_Oui, comme le montre le calcul des addresses sous réseaux: 192.168.1.1/25 => 192.168.1.0 tandis que 192.168.1.130/25 => 192.168.1.128. Donc ils sont bien différents._

## 2. Mise en place d'un VLAN sur le commutateur
### 1) et 4)
VLAN1 :
![](img/TD3/VLAN1.png)

VLAN2 :
![](img/TD3/VLAN2.png)

VLAN3 :
![](img/TD3/VLAN3.png)

VLAN130 :
![](img/TD3/VLAN130.png)

VLAN131 :
![](img/TD3/VLAN131.png)

VLAN132 :
![](img/TD3/VLAN132.png)