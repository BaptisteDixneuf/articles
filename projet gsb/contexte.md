Les rapports de visite sont actuellement gérés à l’aide d’une application Access que les visiteurs utilisent dans les locaux de l’entreprise sur différents postes dédiés à cet effet.
Un projet d’application Web est en cours pour rendre accessible cette gestion à partir de n’importe quel ordinateur. Cependant, l’accès à cette gestion doit être maintenu à l’aide d’une application de bureau, mais l’application Access doit évoluer.
Il a été décidé de développer une application de bureau en java (swing) et de porter la base de données sur SGBD Oracle.

Les fonctionnalités: L’application doit remplir les mêmes fonctionnalités que l’application existante.

#TRAVAIL A RENDRE:

Le projet est divisé en trois étapes que l’on nomme Itérations, durant ces trois « itérations (=SPRINT) », nous avons divers documents à rédiger, dont des jeux d’essais, et du codage a effectuer:

##Les itérations du projet « GSB »:

**Sprint n°1**

- Titre : « Organisation et spécifications »
- Description : organiser le travail en équipe et préparer le premier « livrable »
- Date indicative de remise du livrable : 20/11/2014
- Tâches principales :
	- Organisation de l’équipe
	- Mise en place des outils : Redmine, gestion des versions
	- Tests fonctionnels de l’application existante
	- Recensement des besoins en formation et des moyens de formation
	- MVC en Java, JDBC, Swing, JavaWebStart, Javadoc, …
	- Maquettage en Java
	- Migration de la base de données sous Oracle (script SQL fourni)
	- Modélisation de la base de données (reverse engineering)

**Sprint n°2**

- Titre : « Affichage des visiteurs médicaux »
- Date indicative de remise du livrable : 11/12/2014
- Tâches principales :
	- Organisation de l’application en M.V.C.
	- Spécification, Codage et Tests de la fonctionnalité
	- Documentation et réalisation du livrable

**Sprint n°3**

- Titre : « Suivi des rapports de visite par les visiteurs»
- Date indicative de remise du livrable : 12/03/2015
- Tâches principales :
	- Spécification, Codage et Tests d’une fonctionnalité
	- Documentation et réalisation du livrable


## L’application: ##

**Base de données:**

Le déploiement de la BDD sera effectué sur un SGBD Oracle tournant sur une machine virtuelle VMWare de la ferme de serveurs.
Un script SQL de création de cette base de données vous est fourni. Vous aurez peut-être à retravailler ce script.

**L’exécution de l’application:**

Le déploiement de l’application devra être prévu sur la machine de test de l’équipe sous la forme d’un jar exécutable avec un raccourci sur le bureau de l’utilisateur “2SLAM_2014”.

## ÉVALUATION: ##

Les itérations sont évaluées par analyse des dossiers envoyés sur la FOAD, et par l’analyse de l’application modifiée, déployée sur la plateforme de tests.

De plus, à la fin du projet, chaque étudiant doit remettre le dossier d’examen pour ce PPE :

- la description de la situation professionnelle au format de l’examen
- l’application déployée sur la plateforme de production personnelle de l’étudiant
- la mise à jour du portefeuille de compétences (suivisio et blog)