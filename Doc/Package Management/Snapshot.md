---
icon: history
order: 993
---
Dans l'objectif de gagner en stabilité et en liberté, Nexus propose un système de snapshot qui permet de sauvegarder l'état actuelle des dépendances et de leur version dans l'objectif de restaurer l'état d'un environnement ou pour l'injecter dans un nouvel environnement.

```console
nxs snap
```

Par défaut, le snapshot sera stocké dans un fichier snap.json
<br>
#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] pour spécifier l'environnement a utiliser
[!badge variant="info" text="-f"] ou [!badge variant="info" text="--file"] pour spécifier le fichier de sortie
[!badge variant="info" text="--restore"] pour restaurer un snapshot
[!badge variant="info" text="--force"] pour forcer la restauration