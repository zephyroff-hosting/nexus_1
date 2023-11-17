---
icon: /assets/icons/compilation.svg
order: 991
---
Nexus propose un système de compilation basé sur une intégration de cx_freeze grâce à ma commande compile

```console
nxs compile
```

Les options de compilation sont à retrouver dans le fichier nexus.toml

Avant la compilation, le système va contrôler la présence de toutes les dépendances et leur compatibilité.
<br><br>
#### Options

[!badge variant="info" text="--install"] pour installer ou mettre à jour les dépendances manquantes<br>
[!badge variant="info" text="--nocheck"] pour désactiver la vérification du contrôle de dépendances<br>
[!badge variant="info" text="--dryrun"] pour afficher les informations de compilation sans action<br>
[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour préciser l'environnement qui sera utilisé pour la compilation<br>