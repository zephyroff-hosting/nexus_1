---
icon: file-code
order: 999
---
La commande analyse est une intégration de l'outil pylint qui permet d'analyser le code dans le but de déterminer la qualité du code et de proposer des axes d'améliorations pour se rapprocher des recommandations PEP.
L'analyse va alors nous ressortir la liste des éléments à modifier dans notre code, ainsi qu'une note sur 10 qui sera base en fonction du nombre de problème à corriger.

```console
nxs analyse
```

#### Options

**-e** ou **--exclude** permet d'exclure de l'analyse certains composants.<br>
Par exemple, E0602 pour les undefined variable<br>

**-n** ou **--onlynote** permet d'afficher uniquement la note<br>

**-r** ou **--onlyreport** permet d'afficher uniquement les choses à modifier (sans la note)<br>

**--recursive** permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.<br>