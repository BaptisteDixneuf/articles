## Étape 1: Installation de Python sur la machine Ubuntu ##

Rappel de la mission:

Pour installer Python

- Vous démarrez votre machine seven et vous vous connectez en local avec le compte utilsio, mdp joliverie
- Vous démarrez votre machine ubuntu 
- Paquetages d’installation de Python 
- Vérifiez que l’interpréteur est déjà installé. 
- Pour bénéficier d’un environnement de développement, installer le paquetage “drpython”. Un raccourci sera automatiquement ajouté dans le menu Applications – Développement. 

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_01](https://docs.google.com/document/d/1JrnkFf48wr3Ncvnm-6RGoL7Cbvm0a5Jk3QtUH0BL0dg/edit?usp=sharing)


## Étape 2: Lecture et écriture dans un fichier texte en Python ##

Rappel de la mission:

Pour vous auto-former aux commandes Python permettant de lire et d’écrire dans un fichier texte, vous réalisez un programme lisant le fichier test.txt et vous affichez ce que vous avez lu.

Ensuite vous extrayez la première lettre du premier mot et le deuxième mot pour les afficher.

### Travail à rendre: ###
- synthèse de la gestion des fichiers en Python

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_ETAPE_02](https://docs.google.com/document/d/19FFxB8zE931rztc4zuBgbzwqzz1Xkg7m-ov4jx26sog/edit)
- [DIXNEUF_DRAPEAU_02_MODE_OPERATOIRE](https://docs.google.com/document/d/1-yRe69a2fK8fJv7970hCeWPxcbAdt_8JVr7o84Yy4f4/edit)
- [DRAPEAU_DIXNEUF_CodeSource_Etape_02](https://docs.google.com/document/d/1Ixj6bPjC6zw7_ZPTG-d7pJL_vLiqlj8ZVHdRAN3UVGI/edit)



## Étape 3: Création en SQL des tables dans la base de données ##

Rappel de la mission:

Vous créez les tables SALARIES et PROXY dans la base Oracle. Vous recherchez les ordres SQL pour créer une ligne de la table Proxy pour Oracle . Attention au format date pour Oracle.

### Travail à rendre: ###

- un document pour expliquer ces ordres SQL

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_03](https://docs.google.com/document/d/1asP4oOnwFD_JkujH3ngMLXNANjSyP2c7Do5MaMSAPQk/edit)



## Étape 4: Analyse des fichiers textes de login ##

Rappel de la mission:

Vous analysez les fichiers texte log_proxy_2014-01-xx.txt pour noter les informations que vous pourrez lire dans chaque ligne et dans quel champs de quelle table vous pourrez les enregistrer ou les rechercher.

Exemple: l’adresse IP sera recherchée dans SALARIES et enregistrée dans PROXY.

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_ETAPE_04](https://docs.google.com/document/d/1jY4gdmdMfYHHHJ5oAwALxYcCxlAHZ5EVIqJIfj0ECV4/edit)



## Étape 5: Réalisation des requêtes de validation du jeu d’essai ##

Rappel de la mission:

Vous écrirez les requêtes SQL pour vérifier les 3 demandes du cahier des charges:
- Les sites les plus visités : nombre d’utilisateurs par site 
- La liste des utilisateurs les plus consommateurs: nombre de lignes du fichier de log par utilisateur 
- Qui a consulté tel site, tel jour, à telle heure ?: qui a consulté le site de l’équipe entre 7h et 9h, le 16/01/2014 

### Travail à rendre: ###
- Les trois requêtes SQL

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_ETAPE_05](https://docs.google.com/document/d/1sOm8pyCsMj6qEDSQMQuDSJ8BpzkxUqm3Oti3KtT_VNc/edit)



## Étape 6: Réalisation du script ##

Rappel de la mission:

Vous réaliserez le programme Python. Ce programme lira la liste des enregistrements du proxy dans les fichiers texte log_proxy_2014-01-jj.txt. Ensuite il créera le fichier de script SQL pour créer tous les enregistrements dans PROXY à la date du jj/01/2014.

Dans un premier temps vous pouvez faire saisir le nom du fichier et la date correspondante.

### Travail à rendre: ###
- le code source PYTHON correspondant à cet algorithme
- le script SQL généré pour le journal des logs du 15/01/2014 

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_06](https://docs.google.com/document/d/1UqxFWZSTPxHr83cdnPsD2Er-JoCb-BEPYcfkTyC9Ahs/edit)
- [DIXNEUF_DRAPEAU_ETAPE_06_CODE_SOURCE_PYTHON](https://docs.google.com/document/d/1B3-dFnBJxPm2dVIe7GuGJDfCxkItanES9Dcj3hNbYE0/edit)




## Étape 7: Test du script ##

Rappel de la mission:

Vous réaliserez l’ensemble des tests suivants pour les fichiers log_proxy_2014-01-jj.txt

- Les sites les plus visités : nombre d’utilisateurs par site
- La liste des utilisateurs les plus consommateurs: nombre de lignes du fichier de log par utilisateur
- Qui a consulté tel site, tel jour, à telle heure ? qui a consulté le site de l’équipe entre 7h et 9h, le 16/01/2014 


### Travail à rendre: ###
- le compte rendu de test 

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_ETAPE_07 ](https://docs.google.com/document/d/1WUUaibEo5NsMqrO86cVVrYBqvECxCezK5-R4VisTBLc/edit)



## Étape 8: Rédaction d’un mode opératoire ##

### Travail à rendre : ###
- La réalisation d’un mode opératoire pour l’utilisation du script Python, du script SQL généré et des requêtes de vérification des jeux d’essai 

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_08](https://docs.google.com/document/d/11eKrkITvkdToVuEEzRe1hAIYBLySsqPJyreselYhwVk/edit)




## Étape 9: Première évolution de l’application ##

Rappel de la mission:

Faire une nouvelle version du script Python permettant de gérer les dates et le nom du fichier texte. Le nom du fichier de log sera saisi par l’utilisateur et la date sera extraite du nom du fichier. 

### Travail à rendre: ###

- le code source PYTHON correspondant à cet algorithme. 

### Compte-rendu: ###
- [DRAPEAU_DIXNEUF_ETAPE_9_CODE_SOURCE_PYTHON](https://docs.google.com/document/d/1BpT7FTM5iisPZar39SbhY04ZZKqwXcb63ADqNtUgJuY/edit)




## Étape 10: Deuxième évolution de l’application ##

Rappel de la mission:

Faire une nouvelle version du script Python permettant de prendre en compte les paramètres en ligne de commande. Il sera ainsi possible de lancer le script dans un terminal sous Linux de la manière suivante :

python nomDeVotreScript nomFichierlog NomFichierSQLGenere

### Travail à rendre: ###
- le code source PYTHON correspondant à cet algorithme

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_10_CODE_SOURCE_PYTHON](https://docs.google.com/document/d/1eXUQGmkQ4CFFX6Ry3tC7FWtAHHjsp6ZFdeHY4QxOqPQ/edit)



## Étape 11: Troisième évolution de l’application ##

Rappel de la mission:

Faire une nouvelle version du script Python permettant de traiter plusieurs fichiers et de les passer en paramètre.

python nomDeVotreScript nomFichierlog_2014-01-*.txt NomFichierSQLGenere

### Travail à rendre: ###
- le code source PYTHON correspondant à cet algorithme. 

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_11_CODE_SOURCE_PYTHON](https://docs.google.com/document/d/1Gx68urK5ZXedJumMHHMVRMAfeRpUF-3zzCQikIMZIKo/edit)



## Étape 12: Quatrième évolution de l’application ##

Rappel de la mission:

Le serveur Oracle ne fonctionne plus. Vous n’avez plus accès aux tables Proxy et Salaries. On vous demande en urgence de réaliser les requêtes de l’étape 7 directement avec des scripts python et les fichiers de log.

### Travail à rendre: ###
- le code source PYTHON correspondant à cet algorithme.

### Compte-rendu: ###
- [DIXNEUF_DRAPEAU_ETAPE_12_CODE_SOURCE_PYTHON](https://docs.google.com/document/d/1_tiCLux7jlPeGb17oumP97dOpVxLyUMMir1g4fgh1S0/edit)