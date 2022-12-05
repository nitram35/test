# Spécifications
Ce fichier recense les commandes et explications de chaque spécifications demandées par le commanditaire
## Spécifications fonctionnelles
### SPEC F01 - Consulter les informations d'une UE
**Un utilisateur doit pouvoir consulter pour une UE donnée, toutes les
informations relatives à cette dernière comme le code de l'UE, les différents
créneaux horaires ainsi que les salles qui lui sont associées.**
```console
 node . info <codeUE>
```
### SPEC F02 - Consulter les informations d'une salle
**Un utilisateur doit pouvoir consulter à quel moment de la semaine une
certaine salle est libre. De plus, la capacité maximale d'une salle doit
être indiquée.**
```console
node . 
```
### SPEC F03 - Rechercher une salle libre
**Un utilisateur doit pouvoir rechercher les salles libres pour un
créneau horaire donné.**
```console
node .
```
### SPEC F04 - Exporter son emploi du temps
**Un utilisateur doit pouvoir générer un fichier au format iCalendar entre
deux dates données contenant les cours auxquels il participe, afin de
l'intégrer à son propre logiciel d'agenda.**
```console
node .
```
### SPEC F05 - Statistiques sur les taux d'occupation
**Le système doit générer des visuels permettant de suivre le taux
d'occupation des salles.**
```console
node .
```
### SPEC F06 - Classement des salles par capacité d'accueil
**Le système doit pouvoir générer un classement des salles ordonnées par
capacités d'accueil.**
* Une modification au cahier des charges a été apportée, au lieu d'avoir une liste d'UEs en argument, on a toutes les UEs présentes dans la base de données
```console
node . spec6
```
## Spécifications non fonctionnelles
### SPEC NF01 - Qualité des données
**Le système doit vérifier la qualité des données d'emploi du temps
(redondance, une salle ne peut être utilisée que par un seul professeur
pendant un créneau donné).**
### SPEC NF02 - Portabilité
**Le système doit pouvoir fonctionner sur un matériel informatique plus
ancien.**
### SPEC NF03 - Accessibilité
**Le système doit pouvoir fonctionner dans plusieurs langues (Français,
Anglais, ...)**
```console
node . lang <fr>
```
```console
node . lanf <en>
```
