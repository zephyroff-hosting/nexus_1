---
icon: /assets/icons/provision.svg
order: 992
---
Dans la majorité des repo Python, il est d'usage d'associer un nom de package au profil de son propriétaire. C'est-à-dire que seul celui-ci pourra ajouter ou mettre à jour un package portant ce nom, même si ce même package est supprimé de son profil par l'utilisateur.
Il est donc important de toujours s'assurer que notre nom de package que nous créons est disponible sur le repo souhaité et qu'il le restera pendant le développement de celui-ci.
Pour faciliter cela, Nexus propose une solution qui va provisionner notre nom de package sur notre profil pour éviter de le voir utilisé par un autre utilisateur entre temps.

```console
nxs provisioning {PACKAGE_NAME}
```

Nexus va alors créé un petit package vide, portant la version 0.0.0 et va le publier sur notre profil pour réserver le nom.
Il est possible de préciser l'url du repo avec l'argument **--url**
