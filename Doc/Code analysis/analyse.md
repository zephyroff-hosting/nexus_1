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

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--exclude"] permet d'exclure de l'analyse certains composants.<br>
Par exemple, E0602 pour les undefined variable<br>

[!badge variant="info" text="-n"] ou [!badge variant="info" text="--onlynote"] permet d'afficher uniquement la note<br>

[!badge variant="info" text="-r"] ou [!badge variant="info" text="--onlyreport"] permet d'afficher uniquement les choses à modifier (sans la note)<br>

[!badge variant="info" text="--recursive"] permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.<br>