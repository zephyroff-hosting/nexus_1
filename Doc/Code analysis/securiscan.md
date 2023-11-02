---
icon: file-binary
order: 998
---
La commande securiscan est une intégration de l'outil Bandit qui permet de détecter les problèmes de sécurité courants. Cette option ne remplace pas un réel outil d'analyse de la sécurité de votre code mais propose une premier niveau d'analyse durant votre développement.

```console
nxs securiscan
```

Suite à l'analyse, la commande retournera différents niveaux de détails sur les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.


#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--errors"] affichera les erreurs d'analyse<br>

[!badge variant="info" text="-g"] ou [!badge variant="info" text="--globalmetric"] affichera les totales des métriques suite à l'analyse.<br>
Par exemple, le nombre de faille HIGH, MEDIUM ou LOW<br>

[!badge variant="info" text="-f"] ou [!badge variant="info" text="--filemetric"] affichera les métriques par fichier.<br>

[!badge variant="info" text="-m"] ou [!badge variant="info" text="--allmetric"] affichera l'ensemble des métriques.<br>

[!badge variant="info" text="-d"] ou [!badge variant="info" text="--details"] affichera le détail des résultats comme les erreurs à corriger tels que le nom du fichier, le niveau de criticité, l'emplacement de l'erreur ou encore des liens vers les informations détaillées sur la faille ciblée.<br>

[!badge variant="info" text="-a"] ou [!badge variant="info" text="--all"] affichera l'ensemble des informations.<br>

[!badge variant="info" text="-r"] ou [!badge variant="info" text="--recursive"] permet d'analyser les fichiers .py qui se trouve dans les répertoires.
Cela rendra l'analyse plus longue mais plus complète dans le cas de code complexe.<br>

[!badge variant="info" text="-E"] ou [!badge variant="info" text="--exclude"] permet d'exclure certains fichiers de l'analyse<br>

[!badge variant="info" text="-s"] ou [!badge variant="info" text="--severity"] permet de filtrer par niveau de severity<br>
1: LOW, 2: MEDIUM, 3: HIGH<br>

[!badge variant="info" text="-c"] ou [!badge variant="info" text="--confidence"] permet de filtrer par niveau de confidence <br>
1: LOW, 2: MEDIUM, 3: HIGH<br>