---
icon: desktop-download
order: 997
---
Nexus propose d'installer des packages tout en contrôlant la compatibilité avec les packages déjà installés.

```console
nxs install {PACKAGE_NAME}
```

Dans le cas où nous nous trouvons dans un projet, la commande tentera de trouver un environnement par défaut disponible, sinon fera les installations sur la racine Python.

Dans le cas où nous nous trouvons dans un projet et que nous ne précisons pas de package, la commande va récupérer la liste des dépendances du projet et tenter de les installer.
<br>
#### Options

[!badge variant="info" text="-f"] ou [!badge variant="info" text="--force"] pour forcer l'installation d'un package
[!badge variant="info" text="-r"] ou [!badge variant="info" text="--requirements"] pour installer des packages depuis un fichier requirements
[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement sur lequel installer les packages