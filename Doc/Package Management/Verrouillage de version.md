---
icon: /assets/icons/lock-package.svg
order: 993
---
Pour garantir de toujours utiliser les bonnes versions de dépendances entre environnement, il est possible de verrouiller les versions sur un projet en générant un fichier de lock **nexus.lock**
Grâce à cela, les dépendances qui ont été verrouillées seront installées uniquement dans la version définie dans le fichier de lock.

```console
nxs lock
```

Pour définir les versions de lock, la commande se base sur les versions installées sur l'environnement utilisé.

Il est possible d'ajouter un paramètre le nom des package qui doivent être verrouillés. Dans le cas contraire, l'ensemble des dépendances du projet seront verrouillées.
<br>
#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] permet de spécifier l'environnement utilisé