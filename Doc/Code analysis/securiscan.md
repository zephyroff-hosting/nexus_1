---
icon: 
order: 998
---
La commande securiscan est une intégration de l'outil Bandit qui permet de détecter les problèmes de sécurité courants. Cette option ne remplace pas un réel outil d'analyse de la sécurité de votre code mais propose une premier niveau d'analyse durant votre développement.

```console
nxs securiscan
```

Suite à l'analyse, la commande retournera différents niveaux de détails sur les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.


#### Options

**-e** ou **--errors** affichera les erreurs d'analyse<br>

**-g** ou **--globalmetric** affichera les totales des métriques suite à l'analyse.<br>
Par exemple, le nombre de faille HIGH, MEDIUM ou LOW<br>

**-f** ou **--filemetric** affichera les métriques par fichier.<br>

**-m** ou **--allmetric** affichera l'ensemble des métriques.<br>

**-d** ou **--details** affichera le détail des résultats comme les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.<br>

**-a** ou **--all** affichera l'ensemble des informations.<br>

**-r** ou **--recursive** permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.<br>

**-E** ou **--exclude** permet d'exclure certains fichiers de l'analyse<br>

**-s** ou **--severity** permet de filtrer par niveau de severity<br>
1: LOW, 2: MEDIUM, 3: HIGH<br>

**-c** ou **--confidence** permet de filtrer par niveau de confidence <br>
1: LOW, 2: MEDIUM, 3: HIGH<br>