---
icon: archive
order: 999
---
Pour faciliter l'archivage ou la sauvegarde de nos projets, Nexus propose une solution de sauvegarde qui va archiver et compresser dans un zip l'ensemble de notre projet.

```console
nxs backup
```

La solution va alors récupérer le code du projet, les include_files, la licence, le readme, le changelog et l'ajouter dans une archive.
<br>
#### Options:
[!badge variant="info" text="-q"] ou [!badge variant="info" text="--quality"] pour configurer la qualité de compression (entre 1 et 9)
[!badge variant="info" text="-o"] ou [!badge variant="info" text="--out"] pour définir le nom de l'archive
[!badge variant="info" text="-f"] ou [!badge variant="info" text="--force"] pour forcer l'écriture sur le fichier de sortie