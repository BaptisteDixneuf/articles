# Déroulement du stage #

## MISSION 1 : Découverte  ##
### Le framework PHP CodeIgniter ###

CodeIgniter est un cadre développement (framework) PHP. Il s'agit d'une boite à outils d'aide à la construction de sites web. Son but est de vous permettre d'améliorer le temps de développement de vos projets en vous fournissant un ensemble complet de bibliothèques prenant à leur charge les tâches les plus répétitives, offrant une interface simple et structure logique pour utiliser ces bibliothèques.

- Lecture de la documentation sur [http://codeigniter.fr/user_guide/index.html](http://codeigniter.fr/user_guide/index.html)
- Création d'un mini-projet ( système de login) pour comprendre le framework ( [code dispo ici](https://github.com/BaptisteDixneuf/ci_login) )

### Découverte de SASS  ###
Sass (Syntactically Awesome Stylesheets) est un langage de génération dynamique de feuilles de style

- Correction de bug mineure

### Mise en pratique du versioning ###

Un gestionnaire de version est un système qui enregistre l'évolution d'un fichier ou d'un ensemble de fichiers au cours du temps de manière à ce qu'on puisse rappeler une version antérieure d'un fichier à tout moment.

Réalisation du versionning grâce à GitLab en mode commande: 

- Connexion au serveur en ssh
- Ajout des fichiers pour le commit "git add -A "
- Affichage des fichiers modifiés grâce à "git status"
- Commit des fichiers modifiés " git commit -m "traductions"" ( 15 files changed, 285 insertions(+), 105 deletions(-))
- Pull des modifications réalisées par les autres " git pull origin develop"
- Gestion des conflits
- Ajout des fichiers modifiés suite à la gestion des conflits "git add -A "
- Réalisation d'un second commit ( " git commit -m "fix conflict in get_ask_contact_start")
- Réalisation d'autre pull
- Puis push

## MISSION 2 : Mise en place d'un système permettant l'affichage du site en plusieurs langues ##

### Mise en place de la traduction sur l'ensemble des vues ###

- Repérage des textes en français dans les vues ( + 700 fichiers sur l'ensemble du projet Gladys)
- Création d'un fichier pour chaque langue contenant toutes les traductions du type suivant:
- $lang['language_key'] = "The actual message to be shown";
- On remplace les textes dans les vues par la variable du fichier langue par $this->lang->line('language_key');

### Refonte du Système de notifications ###

Problème rencontré: deux utilisateurs utilisent la plateforme Gladys ( un anglais et un français), si le français publie une info qu'il partage avec l'anglais, l'anglais reçoit une notification en français car c'est l'émetteur qui génère la notification. On souhaite générer la notification dans la langue du destinataire, donc il est nécessaire d'avoir les textes des notifications dans toutes les langues:

- Création d'un nouveau fichiers "hg_multi_lang.php" qui contient les notifications dans toutes les langues
- création d'une fonction qui permet de trouver la langue d'un destinataire en fonction de son id $user_lang = $this->hg_user->get_user_lang(id_destinataire);

### Gestion des mails en diverses langues sur le même principe que les notifications ###


## MISSION 3 : Test fonctionnel ##

### Test fonctionnel des traductions ###
Réalisation de scénario:

- Test invitation
- Création de compte
- Création d'une bulle 
- Création d'une info et réactions
- Agenda
- Upload photo
- Parcours entre les infos
- Création, édition, lien bulles, suppression tag
- Profil ok ( photo, sécurité, fonctions)
- Profil et comptes
- Comptes


### Test fonctionnelle sur IE9 ET IE10 et correction ###
En voici une petite liste:

**Bug de l'an 1970 et 2069**

Quand on change l'échelle sur la Timeline on arrive sur fin décembre 2069 ou début janvier 1970

→ Problème de redirection quand on changeait l'échelle du graphique ( AngularJS)

**Problème de croix ajouté sur les champs de type recherche par internet Explorer sur IE**

-> Modification de feuille CSS (SASS)

**Problème d'affichage du chrono sur IE**

-> Modification des script JavaScript


**+ Test fonctionnelle sur Safari 7 et 6 sur Browserstarck suite à l'analyse d'un taux de rebond élevée sur Google Analytics avec le manager/commercial**


## MISSION 4 : Analyse des systèmes de paiement en ligne ##

###Documentation 



Principe de fonctionnement:

![](https://drive.google.com/uc?id=0BxsdNywXiGpKQ3dMZGpyajlfVzA&authuser=0)


**Avant Installation** ( [https://www.cmcicpaiement.fr/fr/installation/etapes-de-mise-en-oeuvre/index.html](https://www.cmcicpaiement.fr/fr/installation/etapes-de-mise-en-oeuvre/index.html)​) :

* Étape 1 : Constitution du dossier avec la banque
* Étape 2 : Validation du dossier par la banque
* Étape 3 : la réception des informations ( code TPE, Code société)


**Installation:**

* Étape 1 : Lire la documentation technique et général

* Etape 2: Téléchager le kit (https://www.cmcicpaiement.fr/fr/installation/telechargements/kit_telechargeable.aspx)

* Étape 3: Dans le code fourni compléter les variables suivantes:

	* code société ,
	* code TPE,
	* page de retour si validation paiement
	* page de retour si erreur paiement

* Étape 4: Réaliser des tests

**Mise en Production:**

 Lorsque les tests sont finalisés, seul le commerçant peut demander la mise en production.

Pour cela, il doit impérativement écrire à centrecom@e-i.com depuis l'e-mail qu'il a fourni à la signature de son contrat CM-CIC p@iement.
Il doit indiquer :

* son souhait de mise en production,
* le numéro de TPE concerné,
* le code société à passer en production.
* Le numéro de TPE et le code société sont indiqués dans un e-mail reçu par le commerçant suite à la création du contrat.