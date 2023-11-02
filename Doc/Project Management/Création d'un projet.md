---
icon: repo-template
order: 999
---

Nexus propose de créer très rapidement un nouveau projet qui se base sur la structure décrite dans la partie [concept](/Architecture/Concept.md) . Pour cela, on utilise la commande new

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

[!badge variant="info" text="--env"] pour créer un environnement virtuel<br>
[!badge variant="info" text="--noenv"] pour ne pas créer d'environnement virtuel<br>
[!badge variant="info" text="--clear"] pour supprimer le répertoire de l'environnement si non vide<br>
[!badge variant="info" text="--upgradepip"] pour mettre à jour pip au moment de la création<br>
[!badge variant="info" text="--inproject"] pour placer l'environnement dans le répertoire du projet<br>
[!badge variant="info" text="--incache"] pour placer l'environnement dans le répertoire de cache<br>
[!badge variant="info" text="--envpath"] pour spécifier le répertoire de l'environnement<br>
[!badge variant="info" text="--repo"] pour créer un repo dans le projet<br>
[!badge variant="info" text="--norepo"] pour ne pas créer un repo dans le projet<br>