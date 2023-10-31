Nexus propose un système de versioning simplifié pour rapidement prendre en compte une version de package.
Par défaut, la commande sans argument affichera la version actuelle du projet.


```console
nxs version
```

Plusieurs arguments sont possibles pour changer la version du projet actuelle:
- Donner le nom de version souhaité
- Spécifier l'alias (major, minor ou patch). Dans ce cas, le numéro de version sera calculé automatiquement
<br>
En fonction de la configuration du projet, plusieurs autres actions seront réalisés.
- Si un repo est configuré, une nouvelle branche sera créé avec la nouvelle version
- Si le fichier de changelog est configuré, les informations seront demandés pour les ajouter au changelog
