---
icon: 
order: 996
---
Nexus propose un système d'environnement virtuel. 
Un environnement virtuel Python est un espace isolé et autonome dans lequel vous pouvez installer des paquets, dépendances et versions spécifiques de Python pour un projet donné. Ce mécanisme vous permet de maintenir différentes configurations et dépendances de packages pour différents projets, sans interférer avec d'autres environnements Python.

Pour la création de ces environnements, l'outil utilise l'utilitaire virtualenv


L'exécution de la commande sans argument tentera d'ouvrir l'environnement virtuel par défaut

```console
nxs env
```


Pour travailler sur ces projets, Nexus va toujours regarder dans le fichier de configuration du projet si un environnement par défaut est configuré, si c'est le cas il lancera ces actions dessus, dans le cas contraire, il lancera ces actions sur le python racine.