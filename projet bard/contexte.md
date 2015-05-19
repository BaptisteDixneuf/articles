Le projet Parkings Nantes est un projet sur lequel nous sommes partit de zéro, donc pas de ressource ce coup-ci, nous avons donc dû rédiger notre propre cahier des charges.

Nous avons décidé de partager ce projet en deux itérations, une pour le démarrage, avec constitution de l’équipe, réflexion sur ce que nous voulions réaliser, avec la rédaction du cahier des charges.

La deuxième itération étant réservée au codage du site, et, à la création de l’application Androïd reprenant le fonctionnement du site web, avec le maquettage de l’application, la réalisation de l’icône de l’application notamment.

##Définition du besoin

Trouver une place à Nantes est de plus en plus difficile. Beaucoup de bouchons sont liés à une mauvaise circulation au sein des parkings.

Comment fluidifier cette circulation ?

Nous allons répondre à cette demande par la création d’un site web qui permettra de voir en direct (actualisé toutes les 10 minutes) les informations à propos de chaque parking de Nantes comprenant :

* Le nombre de places disponibles dans ce parking
* Le tarif
* La Cartographie (Avec un pointer sur chaque parking)
* Les Heures d’ouverture

##Déploiement de l’application :

**Base de données**
Open date de Nantes Metropole
Fond de carte grâce à l’API de google map ou open street map
Liens vers l’API NANTES:

* [http://data.nantes.fr/?id=441](http://data.nantes.fr/?id=441)
* [http://data.nantes.fr/api/](http://data.nantes.fr/api/)
* [http://data.nantes.fr/donnees/fonctionnement-de-lapi/getdisponibiliteparkingspublics/](http://data.nantes.fr/donnees/fonctionnement-de-lapi/getdisponibiliteparkingspublics/)

**Détails sur l’application**
La partie cliente de l’application sera développée en HTML/ CSS /JS avec les framework Bootstrap pour le CSS et angular JS.

La partie serveur sera l’openData de Nantes, nous utiliserons les données formatées en JSON

##Contraintes concernant l’application :

**Contraintes d’accessibilité et de sécurité**

Application accessible par tous sur le web avec un nom de domaine court. Pas besoin de sécurité étant donné qu’on utilise l’open data de Nantes.

On veut ensuite générer une application mobile.

 **Contraintes de codage**
 
Application “Single Page Application” et responsive.

 **Environnement de développement**
 
* Netbeans -> IDE
* LAMP ou WAMP -> Base de données.
* Serveur de Production.
* Git et Github -> partage du code de l’application pour l’équipe.
* Cordova ou autres services de génération d’appli mobile en HTML / JS .

##Choix du nom :

Nous avons choisi comme nom d’application BARD, reprenant les initiales de nos quatre prénoms (Baptiste, Alexandre, Renaud, David).