---
icon: git-compare
order: 3
---
Nexus propose un système de compilation basé sur une intégration de cx_freeze grâce à ma commande compile

```console
nxs compile
```

Les options de compilation sont à retrouver dans le fichier nexus.toml

Avant la compilation, le système va contrôler la présence de toutes les dépendances et leur compatibilité.
<br><br>
#### Options

**--install** pour installer ou mettre à jour les dépendances manquantes<br>
**--nocheck** pour désactiver la vérification du contrôle de dépendances<br>
**--dryrun** pour afficher les informations de compilation sans action<br>
**-e** ou **--env** pour préciser l'environnement qui sera utilisé pour la compilation<br>