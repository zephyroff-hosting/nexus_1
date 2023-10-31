Nexus propose de créer très rapidement un nouveau projet qui se base sur la structure décrite dans la partie concept. Pour cela, on utilise la commande new

```console
nxs new {PATH}
```

Plusieurs informations seront demandées:
- Le nom du projet
- La version d'origine
- La description du projet
- Le fichier principal
- Le nom de l'auteur
- Le nom du mainteneur
- La licence choisie (les informations nécessaires à la création de la licence)
- Les dépendances nécessaires

Certaines de ces informations comme maintainers ne sont pas obligatoire pour la création du projet.

Une fois les informations renseignées, le projet sera créé et les différents composants tels que l'environnement virtuel et le repo seront créés en fonction des paramètres configurés.
<br>
#### Options

La majorité de ces options se retrouve dans la configuration Nexus met propose d'être dissocié et donc d'être appliqué uniquement sur la création de ce projet.

**--env** pour créer un environnement virtuel<br>
**--noenv** pour ne pas créer d'environnement virtuel<br>
**--clear** pour supprimer le répertoire de l'environnement si non vide<br>
**--upgradepip** pour mettre à jour pip au moment de la création<br>
**--inproject** pour placer l'environnement dans le répertoire du projet<br>
**--incache** pour placer l'environnement dans le répertoire de cache<br>
**--envpath** pour spécifier le répertoire de l'environnement<br>
**--repo** pour créer un repo dans le projet<br>
**--norepo** pour ne pas créer un repo dans le projet<br>