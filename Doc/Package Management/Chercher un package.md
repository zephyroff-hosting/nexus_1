---
icon: search
order: 999
---
Nexus propose une option pour rechercher un package qui pourra être installé par la suite

```console
nxs search {PACKAGE_NAME}
```

Cette commande retourne une liste de package disponible qui correspondent avec leur dernière version disponible et leur description.
L'option [!badge variant="info" text="--strict"] permet d'afficher uniquement les packages dont le nom correspond exactement.