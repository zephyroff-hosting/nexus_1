---
icon: 
order: 994
---
Il est possible que certains packages ont un nom différent entre le nom publié et le nom des module à installer. 
C'est par exemple le cas avec le package py-cpuinfo qui doit être importé avec comme nom cpuinfo.
Dans ce cas, Nexus propose un système d'alias qui permet de faire une correspondance entre le nom publié et le nom d'import

```console
nxs alias
```

Un fichier **.package_alias** sera alors créé à la racine du projet avec l'ensemble des alias
<br>
#### Options

[!badge variant="info" text="-a"] ou [!badge variant="info" text="--add"] pour ajouter un alias
```console
nxs alias --add {IMPORT_NAME} {PACKAGE_NAME}
```
[!badge variant="info" text="-r"] ou [!badge variant="info" text="--remove"] pour supprimer un alias
```console
nxs alias --remove {IMPORT_NAME}
```
[!badge variant="info" text="--windows"] pour ajouter l'alias uniquement pour Windows<br>
[!badge variant="info" text="--linux"] pour ajouter l'alias uniquement pour Linux<br>