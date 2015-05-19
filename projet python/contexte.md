Projet effectué en binôme avec DRAPEAU David.

##CONTEXTE:

Pour être en conformité avec les obligations légales concernant la mise à disposition d’Internet, la société STESIO a mis en place un proxy pour journaliser les accès au web réalisés par ses salariés. A partir de ce journal, le responsable souhaite établir des statistiques comme : 

* les sites les plus visités 
* la liste des utilisateurs les plus consommateurs et dans les cas où cela est nécessaire (enquête de police par exemple) être capable de répondre à une requête du type :
	* qui a consulté tel site,
	*  tel jour, 
	*  à telle heure ?

Le fichier de log du proxy est un simple fichier texte (log_proxy.txt) contenant des informations sur les accès au web comme l’adresse IP, la date, l’heure, la commande HTTP utilisée (GET ou POST) , l’URL des différents éléments constituant la page téléchargée (images, bandeau, …). Ce journal étant d’une part, un fichier texte et d’autre part étant très volumineux, il est difficile à utiliser directement pour répondre facilement à ces besoins.

Le responsable du SI vous demande de créer une base de données sur ORACLE qui contiendra les tables : 
* SALARIES(num, nom, prénom, adresseIP)
* PROXY(num,adresseIP, jour, heure, URL) 

##TRAVAIL A RENDRE:
-> A chaque étape, un fichier ZIP, sous la forme nom1_nom2_Etape_N.zip, contenant les documents demandés.

Note : nom1_nom2 sont les noms des membres du binôme

Documents demandés:

* l’algorithme (en langage naturel) du script qui lit un fichier log_proxy_2014-01-xx.txt et génère le script SQL
* le code source PYTHON correspondant à cet algorithme.
* le script SQL généré
* le code SQL des requêtes
* le compte rendu de test
* un mode opératoire précisant : 
	* l’utilisation du script Python pour générer le script SQL 
	* l’utilisation du script SQL pour peupler la base de données ORACLE 
	* l’utilisation des requêtes d’interrogation de la base de données 

##EVALUATION:

Chaque binôme évalue la réalisation de deux autres binômes : la grille d’évaluation est remplie en testant le jeu d’essai fourni.

