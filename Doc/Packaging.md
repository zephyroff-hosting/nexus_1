---
icon: package
order: 994
---
Nexus propose un système pour faire un package du projet en cours en .whl et/ou .tar.gz pour ensuite être publié sur les repo.

```console
nxs pack
```

Une fois la commande lancée, la système va réaliser un package et le placer dans le répertoire dist du projet.
<br><br>
#### Options

[!badge variant="info" text="--windows"] pour créer un package pour Windows<br>
[!badge variant="info" text="--linux"] pour créer un package pour Linux<br>
[!badge variant="info" text="--sdist"] pour créer un package .tar.gz<br>
[!badge variant="info" text="--d"] ou [!badge variant="info" text="--dryrun"] pour afficher les informations de packaging sans action<br>