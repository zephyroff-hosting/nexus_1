
Dans la majorité des commandes, Nexus tentera de retrouver dans le fichier de configuration du projet si un environnement par défaut est configuré, si c'est le cas il lancera ces actions dessus, dans le cas contraire, il lancera ces actions sur le python racine.

## Définir en environnement par défaut

L'argument **--default** permet de définir l'environnent par défaut.

```console
nxs env --default {ENVNAME}
```


## Désactiver l'environnement par défaut

L'argument **--disable** supprime la mention par défaut sur un environnement.

```console
nxs env --disable {ENVNAME}
```