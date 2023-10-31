---
icon: git-pull-request-draft
order: 998
---
Le fichier nexus.toml contient l'ensemble des informations et des paramètres qui seront nécessaire pour le bon fonctionnement de Nexus.
Ces paramètres sont regroupés par section pour une meilleure compréhension.

Il est possible de retrouver facilement les informations d'un projet avec la commande **project**

```console
nxs project
```
<br><br>
## Description des sections
### Section project

Contient les éléments de base sur la description du projet

**name**: le nom du projet<br>
**version**: la version actuelle<br>
**description**: la description du projet<br>
**mainfile**: le fichier principal qui sera utilisé pour l'exécution du code ou encore la compilation du projet<br>
**requires-python**: les prérequis de version Python
<br><br>
### Section project.metadata

Contient les métadonnées qui seront utilisées pour rendre notre projet publiable.

**authors**: Les auteurs du projet (sous forme de liste)<br>
**maintainers**: Les mainteneurs du projet (sous forme de liste)<br>
**readme**: l'emplacement du fichier readme.md (pour la description principale qui sera utilisée)<br>
**license**: le type de licence utilisée<br>
**license_file**: l'emplacement du fichier de licence<br>
**keywords**: les mots-clés qui seront définis pour rechercher le package dans les repo<br>
**classifiers**: même remarque que keywords<br>
**copyright**: pour spécifier d'éventuels copyright<br>
**changelog**: l'emplacement du fichier de changelog

<br><br>
### Section project.urls

Contient les liens utiles affichés sur les repo

**changelog**: l'url vers le fichier de changelog<br>
**homepage**: l'url vers la page d'accueil du projet<br>
**documentation**: l'url vers la documentation

<br><br>
### Section project.dependencies

Contient l'ensemble des dépendances du projet avec comme format 
NOM_PACKAGE = "VERSION"

Des sous-sections windows et linux sont possibles pour préciser des dépendances spécifiques au système.
<br><br>
### Section project.build

Contient les différentes informations qui seront utiles pour la création de package et la compilation.

**packages**: La liste des packages natif ou à installer nécessaire au projet<br>
**includes**: la liste des modules internes au projet nécessaires<br>
**excludes**: La liste des packages à exclure <br>
**include_files**: La liste des fichiers annexes à intégrer au projet<br>
**optimize**: niveau d'optimisation de la compilation (0 (disabled), 1 or 2)<br>
**no_compress**: booléen qui définit si les dépendances sont dans fichier zip sans compression lors de la compilation<br>
**GUI**: booléen qui définit si le projet a une partie graphique<br>
**icon**: chemin vers le fichier icon qui sera utilisé par l'application compilée

<br><br>
### Section project.wheel

Contient les informations spécifiques pour la création de package

**platforms**: précise la plateforme nécessaire<br>
Une sous-sectoin entry_points contient **console_scripts** qui contient la liste des console_scripts qui seront créés avec notre package.

