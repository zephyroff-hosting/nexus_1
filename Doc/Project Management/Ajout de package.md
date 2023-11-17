---
icon: /assets/icons/add_package.svg
order: 996
---
Pour gérer les dépendances d'un projet, vous pouvez utiliser la commande [!badge variant="info" text="add"] pour ajouter des dépendances au projet.

```console
nxs add {PACKAGE_NAME}
```

Ces dépendances seront alors  ajoutés à la configuration du projet.
<br>
#### Options

[!badge variant="info" text="--windows"] pour ajouter les dépendances uniquement pour Windows<br>
[!badge variant="info" text="--linux"] pour ajouter les dépendances uniquement pour Linux<br>
[!badge variant="info" text="--install"] installer les dépendances ajoutées. Dans ce cas un contrôle de compatibilité entre les dépendances et les packages déjà installés sera effectué pour éviter les conflits<br>
[!badge variant="info" text="--force"] pour forcer l'installation<br>
[!badge variant="info" text="-r"] ou [!badge variant="info" text="--requirements"] pour spécifier un fichier de requirement<br>
[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement sur lequel installer les packages<br>