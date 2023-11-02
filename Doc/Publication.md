---
icon: upload
order: 993
---
Nexus propose une solution pour publier ces packages sur le repo de notre choix (par défaut pypi.org)

```console
nxs publish
```
<br><br>
#### Options

**--url** permet de préciser l'url du repo cible

Une autre méthode pour définir le repo cible est de changer le paramètre **publish.url** dans la configuration Nexus.<br>
Il est également possible de paramétrer le compte qui publie avec le paramètre **publish.username** dans la configuration Nexus.