---
icon: 
order: 997
---
A tout moment, il est possible d'afficher le statut du repo avec la commande [!badge variant="info" text="repo --status"]

```console
nxs repo --status
```

La commande va alors afficher:
- Le nom de la branche active
- L'ID du dernier commit
- La date du dernier commit
- L'auteur
- Le nom du committer
- Le message de commit
- La liste des fichiers qui ont des statuts spécifiques comme des fichiers untracked ou en conflit