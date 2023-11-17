---
icon: /assets/icons/remove-package.svg
order: 996
---
Nexus propose de désinstaller des packages.

```console
nxs uninstall {PACKAGE_NAME}
```

Dans le cas où nous nous trouvons dans un projet, la commande tentera de trouver un environnement par défaut disponible, sinon désinstallera les packages sur la racine Python.

Dans le cas où nous nous trouvons dans un projet et que nous ne précisons pas de package, la commande va récupérer la liste des dépendances du projet et tenter de les désinstaller.
<br>
#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement sur lequel désinstaller les packages