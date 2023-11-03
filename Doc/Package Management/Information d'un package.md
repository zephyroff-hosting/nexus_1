---
icon: 
order: 998
---
Il est possible d'afficher les informations d'un package

```console
nxs info {PACKAGE_NAME}
```

Cette commande affichera:
- Le nom du package
- La dernière version du package
- La description
- Le nom de licence
- L'url de la homepage
- L'arborescence des dépendances
- Les vulnérabilités identifiées
- Indique si le package est installé et sa localisation

Dans ce cas où l'argument est un fichier de package, la commande retournera l'ensemble des métadonnées contenues dans le fichier. 
<br>
#### Options

[!badge variant="info" text="--nodeps"] pour ne pas afficher l'arborescence des dépendances<br>
[!badge variant="info" text="--arbolvl"] pour définir le niveau de recherche de l'arborescence des dépendances<br>
[!badge variant="info" text="--version"] pour afficher la liste des versions disponibles