---
icon: git-pull-request-draft
order: 998
---
La commande clearcode est une intégration de l'outil Black qui permet d'analyser et de corriger le formatage du code.

```console
nxs clearcode
```

Par défaut, la commande va analyser l'ensemble des fichiers .py se trouvant dans le répertoire courant et retourner les modifications dans le prompt.
Il est possible de préciser un ou plusieurs fichiers en particulier pour l'analyse.

#### Options

**--apply** permet d'appliquer les modifications directement sur les fichiers analysés
Cela permettra de corriger le formatage du code sans étape intermédiaire.<br>

**--output** permet de spécifier un fichier de sortie. Les fichiers modifiés seront alors placés dans un autre fichier pour permettre une analyse plus simple des modifications.<br>

**-r** ou **--recursive** permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.<br>

**--fast** permet de faire une analyse rapide du code, qui sera moins précise qu'une analyse complète, mais qui prendra beaucoup moins de temps sur des volumes de code conséquents.<br>


