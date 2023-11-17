---
icon: /assets/icons/repo-restore.svg
order: 988
---
Sans restaurer entièrement une branche, Nexus propose une commande pour restaurer un fichier ou un répertoire d'un ancien commit.

```console
nxs restore {FILE}
```

Par défaut, le fichier sera récupéré depuis le dernier commit et sera restauré à son emplacement d'origine.
<br>
#### Options

[!badge variant="info" text="-d"] ou [!badge variant="info" text="--dest"] pour préciser l'emplacement de la restauration<br>
[!badge variant="info" text="-c"] ou [!badge variant="info" text="--commit"] pour préciser un commit spécifique <br>