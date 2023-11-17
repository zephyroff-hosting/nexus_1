---
icon: /assets/icons/repo-addbranche.svg
order: 994
---
En fonction de la configuration Nexus, les branches seront automatiquement créées en même temps que les changements de version, mais il est possible de rajouter des branches à volonté avec la commande [!badge variant="info" text="branch --add"]

```console
nxs branch --add {NAME_BRANCH}
```

La branche sera alors créée mais ne passera pas en branche active.
<br>
#### Options

[!badge variant="info" text="-S"] ou [!badge variant="info" text="--source"] pour définir la branche source. La nouvelle branche partira alors de cette branche<br>
[!badge variant="info" text="-C"] ou [!badge variant="info" text="--commit"] pour spécifier l'id du commit source. La nouvelle branche partira alors de ce commit