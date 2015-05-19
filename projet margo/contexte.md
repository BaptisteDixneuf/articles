#Objectifs du projet MARGO :

##I-Gestion de projet :

Définir une problématique:
- Connaître les acteurs d’un projet
- Décomposer un projet en tâches, ressources, coûts
- Maîtriser les principaux outils de la gestion de projet
- Optimiser, piloter un projet, anticiper les risques
- Rédiger un cahier des charges

##II- Conception Web :

Concevoir: Les maquettes des pages du futur site MARGO à l’aide de HTM5, CSS3, jQuery
Résultats attendus : Trois itérations = 3 livrables :

| N° Sprint | 	Durée/semaine	| Date début| 	Date fin |	Livrable|
| ----------    | --------------                | ----------        | --------------| ----------  |
|1	|3	|9 septembre	|23 septembre	|Dossier 1
|2	|2	|30 septembre	|7 octobre	|Dossier 2
|3	|5	|14 octobre	|9 décembre	|Dossier 3

##Présentation du contexte

Le centre de formation professionnelle des adultes (MARGO) est un organisme français de formation professionnelle.
Les formations proposées sont sanctionnées par un Titre Professionnel, délivré par le ministère de l’Emploi, et qui est reconnu par les employeurs. Ces titres professionnels sont également accessibles par la validation des acquis de l’expérience (VAE).

Les formations de MARGO sont ouvertes aux demandeurs d’emploi et aux salariés en partenariat avec les organismes publics, les collectivités territoriales, les entreprises (grandes, PME-PMI ou artisans). Les contrats de professionnalisation font aussi partie du dispositif.

MARGO de Nantes a déjà fait appel à un prestataire pour modéliser son SI et réaliser un projet de gestion afin de gérer toutes les informations relatives :

Aux personnes présentes dans le système d’information à savoir : enseignants, techniciens, administratifs, étudiants.
Pour toutes les personnes, on se propose d’enregistrer les nom, prénom, situation de famille et adresse.
Pour les enseignants, les techniciens et les administratifs, on mémorisera les prénoms et dates de naissance de leurs enfants.
Les enseignants et les techniciens peuvent assurer des heures d’enseignement.

* Aux filières d’enseignement (informatique, comptabilité , gestion, commerce) :
* Les matières enseignées (volumes horaires, coefficients.)
* Les classes (exemple : la filière informatique et ses 5 classes : SLAM1, SLAM2, SISR1, SISR2,…)
* Les responsables des filières : un responsable est obligatoirement un enseignant (pas un technicien) dans la filière dont il assume la responsabilité.
* Aux étudiants qui sont affectés à une et une seule classe
* Au nombre d’heures annuelles (par matière) enseignées et assurées par les enseignants ou les techniciens qui peuvent éventuellement donner des cours.
* Autres règles de gestion
* On peut créer des filières sans classe.
* On ne peut pas créer une classe sans qu’elle soit rattachée à une filière.
* On pourra créer des filières sans responsable.
* On pourra créer des étudiants sans les affecter à une classe.
* On pourra créer des personnels sans famille (enfants).
* On pourra créer des classes, des matières, des intervenants sans définir les enseignements.
* Il faudra définir la matière et la classe lors de la création d’un enseignement.
* On pourra définir des enseignements sans les affecter à un enseignant.

Ces règles impliquent la création des constructeurs correspondants.

Travail à faire : Conception d’une application WEB MARGO

##PREMIERE PARTIE (Itération N° 1):

* Rédiger un document décrivant l’existant : Acteurs, tâches et ressources
* Proposer et rédiger une proposition argumentée d’architecture applicative et technique :
* Choix d’une solution SGBD : Comparaison des solutions SGBD proposées pour produire le service
* Dossier de choix présentant les avantages et inconvénients des solutions des « Langages » proposées et les valeurs des critères de choix
* Décomposer votre solution en tâches, ressources et coût
* Elaborer un diagramme de Gantt
* Elaborer un schéma PERT
* Description détaillée de la solution technique nécessaire

##DEUXIEME PARTIE : Cahier des charges (Itération 2)

Ce cahier doit décrire :

* La problématique de la solution
* La définition du projet
* L’analyse de l’environnement
* La structure du projet Web ou intranet proposée
* La maquettage (arborescence, rubriques)
* La charte graphique
* La planification et le budget
* Le cadre juridique et référencement

##TROISIEME PARTIE: MAQUETTAGE DU FUTUR SITE (Itération 3)

Travail à faire : 

* Choix de Template
* Choix d’une charte graphique
* Conception des menus selon les traitements demandés (voir règles de gestion)
* Faire le modèle logique de données
* Créer une base de données ( à partir du modèle logique de données)
* Elaborer trois traitements dynamiques de votre choix (exemples : connexion à l’administration du site, liste des étudiants par classe, liste des professeurs par filière,…..)