---
icon: 
order: 994
---
Nexus propose une solution de vérification du projet. Grâce à cela, plusieurs éléments seront vérifiés:
- Analyse des dépendances du projet: Les dépendances présents dans la configuration du projet seront analysés pour garantir
- Analyse des dépendances inutiles: Une analyse du code et de la configuration du projet sera effectuée pour trouver les dépendances qui seraient configurées mais non utilisées dans le code.
- Analyse des nouvelles dépendances: Une analyse du code et de la configuration du projet sera effectuée pour trouver les dépendances utilisées dans le code mais non configurées dans le projet.
- Vérification des informations de build: Une analyse du code et de la configuration du projet sera effectuée pour trouver les configurations de packaging et de compilation qui seraient incomplètes.

```console
nxs check
```
<br>
#### Options

[!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"] permet de spécifier l'environnement utilisé