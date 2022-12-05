# GL02_A22_grpPython - Contexte SRU

Utilitaire en invite de commande pour l'Université centrale de la république de Sealand qui souhaite faciliter la gestion de ses locaux et l'organisation de ses usagers.

## Contributeurs
Etudiants de l'UTT, groupe Python - A22
- [Martin Gandon](mailto:martin.gandon@utt.fr)
- [Louis Duhal-Berruer](mailto:louis.duhal_berruer@utt.fr)
- [Louis Give](mailto:louis.give@utt.fr)
- [Marielle Charon](mailto:marielle.charon@utt.fr)


## Installation & exécution
Ce programme nécessite Node.js > 15.0.0 et npm > 6.0.0 pour être exécuté.
Aide pour [Installer '**nodejs**'](https://nodejs.org/fr/download/)

Ouvrez le dossier contenant le projet et vérifiez que le fichier **package.json** est présent puis, suivez les instructions ci-dessous :

 ### Installez les dépendances avec npm
 ```console
npm install
```
### Construisez le projet
```console
npm run build
```  
**Un unique fichier JavaScript a été produit, il se trouve dans ./dist/bundle.cjs. Le programme peut être exécuté des façons suivantes :**

```console
node ./dist/cm.cjs
```

ou

```console
npm start
```

ou plus simplement

```console
node .
```
### Créer un exécutable (distribuable)

```console
npm make
```

**Trois binaires ont été créés dans le répertoire bin, un pour Windows, un pour macos et un pour Linux, ils peuvent être ensuite distribués aux utilisateurs finaux**
## Développement

### Installez les dépendances

```console
npm install
```

### Lancer le mode de développement

```console
npm run dev
```

### Exécutez pour tester vos modifications

```console
node .
```

## Tests unitaires
### Lancez les tests avec :
```console
npm run test
```
## Choix Technique

 1. **Commander API** : aucune différence d'API avec Caporal, mis à jour régulièrement, communauté importante
 2. **Chalk API** :  expressive API
 3. **i18n.ts** : permet d'améliorer l'expérience développeur 
 4. **pkg** : permet de créer un binaire variable
 5. **esbuild** : compilateur javascript
 6. **ics** : serialiseur/déseraliseur au format ICalendar
 7.  **vitest** : Utiliser pour les tests unitaires
