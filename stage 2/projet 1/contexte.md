##1. Introduction

VIF a développé en interne une petite application web permettant de gérer la saisie et la validation des jours de congés/récupérations. L’objectif du stage est de mettre en place une synchronisation des demandes de congés ainsi que des jours de congés validés avec les Agendas Google des employés.

La première phase du projet consistera à déterminer le mode de fonctionnement à mettre en place (création des événements de manière synchrone/asynchrone, avec ou sans réplication) et le langage de programmation à utiliser (Code PHP/Java avec déploiement en interne ou sur Google AppEngine).

Le développement et la mise en production seront ensuite effectués.


##Présentation de l’existant

[http://intranettest.vif.fr/conges/conges.phtml]()

L’outil a été développé en PHP et est accessible sur l’intranet interne de la société (serveur Apache Httpd 2.2, PHP 5.1.6).

Les utilisateurs sont identifiés à l’aide d’un système d’authentification simple ($PHP_AUTH_USER).

Toutes les données (logins utilisateurs et informations relatives aux congés) sont stockées en base PostgreSQL.
Nom de base : maint
Tables : astreinte, conges, conges_recup, recup, solde et utilisateur

##Ressources utiles
API Google pour PHP
[https://developers.google.com/google-apps/calendar/downloads]()

API Google pour Javascript
[https://developers.google.com/api-client-library/javascript/start/start-js]()

API Google pour Java
[https://code.google.com/p/google-api-java-client/]()

Google Calendar API reference
[https://developers.google.com/google-apps/calendar/v3/reference]()

Upgrade PHP 5.2/5.3
[http://wiki.centos.org/HowTos/PHP_5.1_To_5.2]()



