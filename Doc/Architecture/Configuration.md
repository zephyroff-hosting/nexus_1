---
icon: 
order: 997
---
La configuration Nexus est un ensemble de paramètres qui sont applicables à l'ensemble des projets et qui permettent de contrôler certains comportements comme les environnements virtuels, les repos ou encore l'affichage de logs.

Pour voir l'ensemble des paramètres configurés, il suffit d'appeler la commande **config**

```console
nxs config
```

Il existe 2 types de paramètres:
- Les paramètres booléen: Qui sont modifiables simplement en donnant le nom du paramètre dans l'appel de la commande

```console
nxs config {PARAMETER}
```

- Les paramètres à valeur: Qui sont modifiables en donnant le nom du paramètre suivi de la valeur souhaitée (en comptant que certains paramètres doivent être des nombres)

```console
nxs config {PARAMETER} {VALUE}
```
<br>
### Désactivation de paramètre

Pour des besoins ponctuels, il est possible de désactiver ces paramètres avec l'argument **--disable**. 
Ces paramètres seront alors encore présent dans la configuration mais ne seront plus appliqué jusqu'à réactivation.

```console
nxs config --disable {PARAMETER}
```

et de les réactiver avec l'argument **--enable**

```console
nxs config --enable {PARAMETER}
```
<br>
### Recharger la configuration

Dans le cas de configuration corrompue ou erronée, il est possible de recharger la configuration avec ces paramètres par défaut avec l'argument **--reload**

```console
nxs config --reload
```
<br>
### Description des paramètres

Ces paramètres sont regroupés en catégories (general, virtualenvs, logs, project, publish, repo).
Chacun agit sur un ou plusieurs composants.
<br>
#### general
[!badge variant="info" text="cache-dir"] : Défini l'emplacement du répertoire de cache
[!badge variant="light" text="proxy"] : Configuration d'un proxy pour les commandes ayant besoin d'internet
[!badge variant="ghost" text="threading"] : Active l'utilisation de multi-thread pour les traitements
[!badge variant="ghost" text="threadmax"] : Défini le nombre maximum de thread parallèle
<br>
#### virtualenvs

<br>
#### logs

<br>
#### project

<br>
#### publish

<br>
#### repo