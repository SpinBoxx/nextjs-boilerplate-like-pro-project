# Nextjs Boilerplate

- [Nextjs Boilerplate](#nextjs-boilerplate)
  - [Tools installed](#tools-installed)
  - [Installation et configuration](#installation-et-configuration)
    - [BiomeJS](#biomejs)
      - [Triage automatique des imports au save d'un fichier](#triage-automatique-des-imports-au-save-dun-fichier)

## Tools installed

Voici la liste des lib, outils installés sur le projet : 

- BiomeJS
- TailwindCSS

## Installation et configuration


### BiomeJS 

BiomeJS est le formatter, linter et analyizer de cette application. Voir [documentation](https://biomejs.dev/)

Il faut ensuite ajouter Biome comme extension VScode et ensuite activer Biome comme formatter par défaut de VSCode, pour cela : 

- Allez dans les parametres VScode
- Tapez `formatter` et choisir Bione dans la liste déroulante 

#### Triage automatique des imports au save d'un fichier

Il est possible avec Biome de trier les imports selon une config de base de Biome. Pour cela, il faut ajouter dans le fichier settings.json de VScode : 

```  
"editor.codeActionsOnSave":{
  "source.organizeImports.biome": "explicit"
}
```