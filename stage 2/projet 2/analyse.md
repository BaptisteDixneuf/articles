##1. Introduction

VIF accueille régulièrement des stagiaires. Chaque stagiaire dispose d’un ordinateur et d’un accès au réseau intranet de la société, ce qui pose quelques problèmes de sécurité. VIF souhaite mettre en place une gestion des accès plus rigoureuses. Pour cela, le trafic du  VLAN “Stagiaire” passera par un pare-feu configuré avec IPTABLES pour gérer les accès. 

L’objectif du projet est de mettre en place une édition des règles IPTABLES plus facile grâce à une interface web.

##2. Schéma Réseau

Voici un petit schéma résumant la situation:

Avant :

![](https://drive.google.com/uc?id=0BxsdNywXiGpKQWQ0a1pZZF9tSHM&authuser=0)

Après :

![](https://drive.google.com/uc?id=0BxsdNywXiGpKTll2YjJxekFOdDg&authuser=0)




###2.1 Avantages Firewall

* Filtrage IP :
	* Idée : contrôler les paquets IP autorisés à atteindre un hôte 
 	* Intérêt : sécuriser un hôte de façon globale (au niveau réseau)

### 2.2 Inconvénients Firewall

* Goulet d’étranglement réseau 

## 3.Iptables

La solution retenue pour gérer les règles du firewall est Iptables.

###3.1 Explications
Iptables fonctionne selon un système de tables, ces tables sont composées de chaîne. 

Elle est composée de trois sortes de chaîne :
* INPUT : Permet d'analyser les paquets entrants. Si le paquet est adressé au poste, il est confronté au filtre INPUT.
* FORWARD : Permet d'analyser et d'autoriser les trames à passer d'une interface à une autre, seulement dans le cadre d'une interface réseau servant de passerelle.
* OUTPUT : Permet d'analyser les paquets sortants. Si le paquet sort du poste, il passera par la chaîne OUTPUT.


### 3.2 Configuration du pare-feu

Nous allons configurer notre pare-feu de la manière suivante :
* On bloque tout le trafic entrant par défaut.
* On autorise au cas par cas : le trafic appartenant ou lié à des connexions déjà établies et le trafic à destination des serveurs (web, ssh, etc.) que nous souhaitons mettre à disposition.


###3.3 Exemple de lignes FORWARD


```
 iptables -t filter -A FORWARD -i eth0 -o eth2 -p tcp -s 10.224.14.9 -d 128.15.2.221 --dport 8080 -m state --state NEW,ESTABLISHED  -j ACCEPT 
```

Partie identique → Partie Bleue

* -i : --in-interface  →  Interface INPUT → input name, network interface name
* -o : --out-interface → Interface OUTPUT →  output name, network interface name 
* -p → protocole
* -s : --source   → adresse IP
* -d --destination  ->   adresse IP
* Un port
	* --dport 
* Plusieurs ports
	* -m -multiports --dports

##4. Utilisation 

Diagramme Scénario:
![](https://drive.google.com/uc?id=0BxsdNywXiGpKaEYzZ3Y5YkdkMkU&authuser=0)
Les fonctionnalités retenues sont :

*  Ajout d’une iptable
* Modification une iptable
* Suppression d’une iptable
* Duplication d’une iptable
* Sélection d’une/plusieurs iptables(s) pour les dupliquer/supprimer
* Filtrage de données
 



## 5. Prototype d’interface utilisateur

L’interface retenue est une ”Single Page Application”.
![](https://drive.google.com/uc?id=0BxsdNywXiGpKT2JjWXk0eEdMaVU&authuser=0)


Lors de l’ajout/Edition d’une iptable, une fenêtre modal s’ouvre.

![](https://drive.google.com/uc?id=0BxsdNywXiGpKN2FSaW9RVU01ckE&authuser=0)


Example d’interface: 

* Exemple filtrage :  http://bazalt-cms.com/ng-table/example/4
* Exemple edition : http://bazalt-cms.com/ng-table/example/16







##6. Langages

###6.1 Côté Client

Coté client, on souhaite avoir une application simple et rapide . Les ajouts, les modifications et les suppressions d’iptables doivent se réalisent facilement. On ne souhaite pas avoir enchaînement de formulaires, pour cela, on a choisit: 

* HTML/CSS → Application disponible depuis un navigateur ( pas d’installation)
* JavaScript avec le framework AngularJS → pour la réactivité

###6.2 Côté Serveur

Côté Serveur, on a choisit :

PHP pour répondre aux :

→ Fonctionnalités: 

Fonction 1:

* Récupérer le fichier
* Parser les données facilement
* Afficher les données au format JSON

Fonction 2: 

* Traiter les données reçues
* Générer un nouveau fichier Iptables
* Modifier le fichier iptables et appliquer les règles iptables sur la machine



