---
icon: package
order: 995
---
Nexus propose un système pour faire un package du projet en cours en .whl et/ou .tar.gz pour ensuite être publié sur les repo.

```console
nxs pack
```

Une fois la commande lancée, la système va réaliser un package et le placer dans le répertoire dist du projet.
<br><br>
#### Options

**--windows** pour créer un package pour Windows<br>
**--linux** pour créer un package pour Linux<br>
**--sdist** pour créer un package .tar.gz<br>
**--d** ou **--dryrun** pour afficher les informations de packaging sans action<br>