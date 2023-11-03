---
icon: database
order: 987
---
Pour gagner en réactivité et en temps de traitement, Nexus propose un système de cache pour sauvegarder les informations sur les packages. Ces informations pourront alors être réutilisées par les autres commandes sans avoir besoin de réinterroger les repos.

Pour connaître la capacité du cache à l'instant T, il suffit d'appeler la commande [!badge variant="info" text="cache"]

```console
nxs cache
```

Celle-ci retournera l'espace de stockage utilisé, le nombre de package et le nombre de version différente stockés.

Il est également possible de lister les packages et leur version stockée dans le cache avec l'argument [!badge variant="info" text="-l"] ou [!badge variant="info" text="--list"]