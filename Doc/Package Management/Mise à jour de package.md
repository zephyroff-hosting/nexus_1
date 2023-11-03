---
icon: 
order: 995
---
La solution propose de mettre à jour l'ensemble ou une partie des packages d'un environnement.

```console
nxs update {PACKAGE_NAME}
```

Dans le cas où nous nous trouvons dans un projet, la commande tentera de trouver un environnement par défaut disponible, sinon mettra à jour les packages sur la racine Python.

Dans le cas où nous nous trouvons dans un projet et que nous ne précisons pas de package, la commande va récupérer la liste des dépendances du projet et tenter de les mettre à jour.
<br>
#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement sur lequel mettre à jour les packages.
[!badge variant="info" text="-d"] ou [!badge variant="info" text="--dryrun"] pour permettre de tester les mises à jour sur un environnement isolé.
[!badge variant="info" text="-f"] ou [!badge variant="info" text="--full"] pour mettre à jour l'ensemble des packages d'un environnement.