---
icon: /assets/icons/remove_package.svg
order: 995
---
Pour gérer les dépendances d'un projet, vous pouvez utiliser la commande [!badge variant="info" text="remove"] pour supprimer des dépendances au projet.

```console
nxs remove {PACKAGE_NAME}
```

Ces dépendances seront alors supprimées à la configuration du projet.
<br>
#### Options

[!badge variant="info" text="--windows"] pour supprimer les dépendances uniquement pour Windows<br>
[!badge variant="info" text="--linux"] pour supprimer les dépendances uniquement pour Linux<br>
[!badge variant="info" text="--uninstall"] désinstaller les dépendances supprimées<br>
[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement sur lequel désinstaller les packages<br>