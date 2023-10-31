La commande securiscan est une intégration de l'outil Bandit qui permet de détecter les problèmes de sécurité courants. Cette option ne remplace pas un réel outil d'analyse de la sécurité de votre code mais propose une premier niveau d'analyse durant votre développement.

```console
nxs securiscan
```

Suite à l'analyse, la commande retournera différents niveaux de détails sur les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.


#### Options

**-e** ou **--errors** affichera les erreurs d'analyse

**-g** ou **--globalmetric** affichera les totales des métriques suite à l'analyse.
Par exemple, le nombre de faille HIGH, MEDIUM ou LOW

**-f** ou **--filemetric** affichera les métriques par fichier.

**-m** ou **--allmetric** affichera l'ensemble des métriques.

**-d** ou **--details** affichera le détail des résultats comme les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.

**-a** ou **--all** affichera l'ensemble des informations.

**-r** ou **--recursive** permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.

**-E** ou **--exclude** permet d'exclure certains fichiers de l'analyse

**-s** ou **--severity** permet de filtrer par niveau de severity
1: LOW, 2: MEDIUM, 3: HIGH

**-c** ou **--confidence** permet de filtrer par niveau de confidence 
1: LOW, 2: MEDIUM, 3: HIGH