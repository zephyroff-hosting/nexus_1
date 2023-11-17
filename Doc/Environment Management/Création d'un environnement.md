---
icon: /assets/icons/env-newsvg
order: 998
---
Pour la création d'un environnement virtuel, nous utilisons l'argument **env --create**

```console
nxs env --create {ENVNAME}
```

Il faudra à minima préciser le nom de l'environnement

Dans la [configuration Nexus](/Architecture/Configuration.md), il existe des paramètres qui sont utilisés pour définir le comportement lors de la création des environnements.
<br><br>
#### Options

[!badge variant="info" text="-d"] ou [!badge variant="info" text="--default"] pour définir ce nouvel environnement comme l'environnement par défaut<br>
[!badge variant="info" text="--withoutdeps"] pour définir si les dépendances du projet doit être installés au moment de la création de l'environnement<br>
[!badge variant="info" text="--clear"] pour définir si le dossier de l'environnement doit être nettoyer si non vide lors de la création<br>
[!badge variant="info" text="-C"] ou [!badge variant="info" text="--cache"] pour forcer la création de l'environnement dans le dossier de cache<br>
[!badge variant="info" text="-p"] ou [!badge variant="info" text="--prompt"] pour définir le prompt dans l'environnement<br>