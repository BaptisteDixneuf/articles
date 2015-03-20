## Projet Java – Mission 01 ##
Binômes de l’équipe:

- Binôme 01 -> DIXNEUF Baptiste et DRAPEAU David
- Binôme 02 -> JAUNASSE Alexandre et BONIN Alexis

### Mission 1 : amélioration de l’ergonomie /Découverte (pas plus d’une demi-journé ###e)
- Rappel de la mission:
- Difficulté : *
- Résultats attendus :
	- Le projet 
	- Le compte-rendu doit contenir en plus:
		- une copie d’écran montrant que vous avez accès à la documentation
		- les lignes de code ajoutées ou modifiées
		- aucun rapport de test formel n’est demandé

### Préparation de la mission ###
- Constituez les équipes et les sous-équipes. 
- Affectez les missions aux sous-équipes. 
- Installez l’application et la base de données et testez-la. 
- Étudiez le code. 
- Supprimez les import inutiles. 
- Insérez des commentaires dans le code de la classe VueAdresse_init 

Vous pourrez vous inspirer des règles concernant les commentaires énoncées dans le document GSB-ApplisWebPHP-NormesDevlpt.doc p. 12-14. 

### Documentation ###

Vérifiez que vous avez accès à une documentation java en local.

### Amélioration de l’application ###

Nous souhaitons que l’ergonomie de l’application soit améliorée :

- Rajoutez un bouton “Quitter” qui permet de sortir de l’application. 
- Faites en sorte que l’appui sur le touche “Entrée” lorsque l’on est dans le champ de saisie de l’identifiant, déclenche la validation. 
- Faites en sorte que l’appui sur le touche “Escape” lorsque l’on est dans le champ de saisie de l’identifiant, déclenche l’annulation.

Compte-rendu:

- Compte-rendu binôme 01: [Equipe5_mission1_DRAPEAU_DIXNEUF](https://docs.google.com/document/d/1ifnEermN_N55Dlzc63kblkF6Ri_xdd97x7rF9GfMMDQ/edit)
- Compte-redu binôme 02: [Groupe5_Mission1_Bonnin_Jaunasse](https://docs.google.com/document/d/1isaSZHyq4fPBOwPAyxmi3mBFRnULzvwK0FiDFBCFPdQ/edit#)


## Projet Java – Mission 02 ##

Binômes de l’équipe:

- Binôme 01 -> DIXNEUF Baptiste et DRAPEAU David
- Binôme 02 -> JAUNASSE Alexandre et BONIN Alexis (Seul le binôme 02 s’occupait de cette mission)

### Mission 2 : amélioration fonctionnelle /Précédent-suivant (de 1 à 1,5 journée) ###

- Rappel de la mission:
- Difficulté : *
- Résultats attendus :
- Le projet 
- Le compte-rendu
- en plus, le principe de la solution. 

### Amélioration fonctionnelle ###

Nous souhaitons pouvoir faire défiler les adresses avec des touches Suivant/Précédent. Nous vous demandons de présenter oralement le principe de votre solution au professeur avant de coder. Notez que le code existant va être impacté de façon assez notable.

### Compte-rendu: ###
- Compte-rendu binôme 02 (seul ce binôme travaillé sur cette mission): [equipe5_mission2_compte_rendu_bonnin_jaunasse](https://docs.google.com/document/d/1DsVxk2bPHdqTpM5B716bo4OiX2yFH3iMSoSroYN1iwU/edit)


## Projet Java – Mission 03 ##
Binômes de l’équipe:

- Binôme 01 -> DIXNEUF Baptiste et DRAPEAU David
- Binôme 02 -> JAUNASSE Alexandre et BONIN Alexis (Seul ce binôme travaillait sur cette mission)

### Mission 3 : amélioration fonctionnelle -Tri (de 0,5 à 1 journée) ###

Rappel de la mission:
- Difficulté : **
- Résultats attendus :
- Le projet 
- Le compte-rendu avec une maquette ou une copie d’écran de la vue. 

### Amélioration fonctionnelle ###

Nous souhaitons pouvoir faire défiler les adresses dans un certain ordre. 
- L’ordre initial d’insertion dans la table, 
- L’ordre trié par identifiant des adresses, 
- L’ordre trié par nom de ville. 
- De plus on devra pouvoir choisir entre un ordre décroissant de ces clés de tri. 

On appréciera de la pertinence des contrôles graphiques choisis.

### Compte-rendu: ###

- Compte-rendu binôme 02 (seul ce binôme travaillait sur cette mission) :[groupe5_mission3_bonnin_jaunasse](https://docs.google.com/document/d/1_JtHtUWLYZpmyYCs-8tdh2w0gV7TYPDewxBphlvOj48/edit)
 


## Projet Java – Mission 04 ##
Binômes de l’équipe:

- Binôme 01 -> DIXNEUF Baptiste et DRAPEAU David (Seul notre binôme travaillait sur cette mission)
- Binôme 02 -> JAUNASSE Alexandre et BONIN Alexis

### Mission 4 : Ajout fonctionnelle – Gestion des villes (de 1,5 à 2 journées) ###
Rappel de la mission:
- Difficulté : **
- Résultats attendus :
- Le projet 
- Le compte-rendu 

### Ajout fonctionnel ###

Dans un premier temps, nous souhaitons concevoir une interface qui permet de choisir une ville suivant le code postal.

L’objectif est ensuite d’utiliser cette interface pour la saisie des villes des adresses. Il n’y aura ainsi aucune erreur de saisie dans les villes et celles-ci seront toujours au même format (majuscules, tirets …

Dans la description de votre démarche de solution, vous préciserez bien les impacts à tous les niveaux de cet ajout fonctionnel.

Un choix pertinent des contrôles graphiques utilisés est attendu.

### Les scénarios ###

Les scénarios suivants décrivent le comportement de l’interface.

#### Scénario nominal : ####
1) l’utilisateur saisit 44310 et valide

2) le système affiche une liste de villes (triée par nom) correspondant à ce code postal, en l’occurrence :

- LA LIMOUZINIERE
- SAINT-COLOMBAN
- SAINT-LUMINE-DE-COUTAIS
- SAINT-PHILBERT-DE-GRAND-LIEU

3) l’utilisateur choisit une ville.

4) le système affiche le code postal de la ville

5) l’utilisateur quitte l’interface

#### Scénario alternatif 1 : ####
1) l’utilisateur saisit 443 et valide

2) le système affiche une liste de villes (triée par nom) dont le code postal commence par ces chiffres, en l’occurrence :

- ARTHON-EN-RETZ
- BELIGNE
- BOUGUENAIS
- … 
- LA LIMOUZINIERE
- SAINT-COLOMBAN
- SAINT-LUMINE-DE-COUTAIS
- SAINT-PHILBERT-DE-GRAND-LIEU

3) retour 3 scénario nominal

####  Scénario erreur1 :  ####
1) l’utilisateur ne saisit rien et valide

2) le système n’affiche rien

3) l’utilisateur quitte l’interface

####  Scénario erreur2 :  ####
1) l’utilisateur ne saisit rien et valide

2) le système n’affiche rien

3) retour 1 scénario nominal

### Compte-rendu: ###

- Compte-rendu binôme 01 (seul notre binôme travaillait sur cette mission) :[Equipe5_mission4_DRAPEAU_DIXNEUF](https://docs.google.com/document/d/117r6YsFOqdePWtf1ZmgbPbQDOn0Kxv6GAisWclhBMUE/edit)


## Projet Java – Mission 05 ##
Binômes de l’équipe:

- Binôme 01 -> DIXNEUF Baptiste et DRAPEAU David
- Binôme 02 -> JAUNASSE Alexandre et BONIN Alexis

Sur cette mission, nous avons travaillé en quatuor!

### Mission 5 : Fusion des applications / Gestion des adresses – Gestion des villes (de 1 à 1,5 journées) ###

Rappel de la mission:
- Difficulté : *
- Résultats attendus :
- Le projet 
- Le compte-rendu 

### Fusion ###
Description succincte :

Les champs code postal et ville sont toujours en grisé (disabled). Lorsque l’on ajoute ou modifie une adresse, un bouton “Choisir la ville devient enabled.

Lorsque l’on clique sur ce bouton, la fenêtre modale de choix d’une ville s’affiche.

Si l’on choisit de valider le choix d’une ville, il y a retour à l’écran de gestion des adresses avec les informations de la ville choisie.

Si l’on choisit d’annuler le choix d’une ville, on revient à l’écran de gestion des adresses sans modification des informations de la ville choisie.

### Rédaction de la démarche ###

Dans un premier temps vous allez rédiger votre ébauche de solution. Pour cela :

- Listez les tâches à réaliser et leurs liens de précédence.
- Évaluiez le temps pour chaque tâche
- Faites une répartition des tâches et évaluez le temps qu’il faudra à votre équipe pour réaliser la fusion.

### Codage de la solution ###

### Compte-rendu de l’équipe: ###
[Equipe5_mission5_DRAPEAU_DIXNEUF_JAUNASSE_BONNIN](https://docs.google.com/document/d/19lu9LmyexWLh3TyxFcmacln8r3cDA_gSKawOALTrl9s/edit)