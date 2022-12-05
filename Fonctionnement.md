# Fonctionnement
Ce document présente le fonctionnement de notre application.

## Données
Le jeu de données initialement données pour le projet est dans le dossier `data`. Il est constitué de sous-dossiers classés par tranche alphabétique contenant un unique fichier chacun `edt.cru`. 
Exemple : `data/AB/edt.cru` comprend toutes les infos concernant les UEs commençant par A ou B.

## Parseur & Système de base de données
La totalité des fonctionnalités du projet (Spécifications) repose sur notre parseur `src/parser.js` et notre système de base de données `src/db.js`.

Peu importe les fonctionnalités, il faut que nous puissions extraitre les différents types de données présents dans un fichier `edt.cru`. 

Ainsi, pour chaque Spécificiation nous pouvons importer la Base de données de plusieurs façons :
 - `node . db import <path>` qui importe la totalité des données d'un dossier
 - `node . db import --filter=<UE1>,<UE2>,...` qui importe seulement les données des UEs choisis
 
Le parseur va permettre **de "découper" le fichier de données en un ensemble d'objets crées à partir des classes définies dans `src/models`**. Cet ensemble constituera le jeu de données nécessaire au fonctionnement de la Spécification.

La commande `node . db info`permettra de connaître le nombre d'UEs présentes dans la base de données

Nous pouvons également supprimer la Base de données de plusieurs façons :
 - `node . db drop` qui efface la base de données
 - `node . db delete --filter=<UE1>,<UE2>,...` qui efface seulement les données des UEs choisies

