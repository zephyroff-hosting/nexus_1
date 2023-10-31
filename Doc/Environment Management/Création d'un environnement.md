
Pour la création d'un environnement virtuel, nous utilisons l'argument **env --create**

```console
nxs env --create {ENVNAME}
```

Il faudra à minima préciser le nom de l'environnement


Dans la configuration Nexus, il existe des paramètres qui sont utilisés pour définir le comportement lors de la création des environnements

virtualenvs.create: Détermine si un environnement virtuel est créé lors de la création d'un projet Nexus
virtualenvs.clear: Détermine si le dossier de l'environnement doit être nettoyer si non vide lors de la création
virtualenvs.upgradepip: Détermine si pip doit être mis à jour lors de la création
virtualenvs.in-project: Détermine si l'environnement doit être créé dans le répertoire du projet (sinon est créé dans le répertoire cache-dir)
virtualenvs.symlinks: Détermine si l'environnement fait des liens symboliques ou copie les exécutables Python
virtualenvs.system-site-packages: Détermine si l'environnement peut utiliser le site-packages du système
virtualenvs.foldername: Détermine le nom du répertoire des environnements virtuels


#### Options

**-d** ou **--default** pour définir ce nouvel environnement comme l'environnement par défaut

**--withoutdeps** pour définir si les dépendances du projet doit être installés au moment de la création de l'environnement

**--clear** pour définir si le dossier de l'environnement doit être nettoyer si non vide lors de la création

**-C** ou **--cache** pour forcer la création de l'environnement dans le dossier de cache

**-p** ou **--prompt** pour définir le prompt dans l'environnement