---
icon: 
order: 997
---
La configuration Nexus est un ensemble de paramètres qui sont applicables à l'ensemble des projets et qui permettent de contrôler certains comportements comme les environnements virtuels, les repos ou encore l'affichage de logs.

Pour voir l'ensemble des paramètres configurés, il suffit d'appeler la commande **config**

```console
nxs config
```
<br>
Il existe 2 types de paramètres:

- ***Les paramètres booléen***: Qui sont modifiables simplement en donnant le nom du paramètre dans l'appel de la commande

```console
nxs config {PARAMETER}
```

- ***Les paramètres à valeur***: Qui sont modifiables en donnant le nom du paramètre suivi de la valeur souhaitée (en comptant que certains paramètres doivent être des nombres)

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
[!badge variant="info" text="cache-dir"] : Défini l'emplacement du répertoire de cache<br>
[!badge variant="info" text="proxy"] : Configuration d'un proxy pour les commandes ayant besoin d'internet<br>
[!badge variant="info" text="threading"] : Active l'utilisation de multi-thread pour les traitements<br>
[!badge variant="info" text="threadmax"] : Défini le nombre maximum de thread parallèle
<br>

#### virtualenvs

Ces paramètres seront utilisés pour la création d'un environnement virtuel.

[!badge variant="info" text="virtualenvs.create"] : Création d'un environnement virtuel au moment de la création ou de l'initialisation d'un projet<br>
[!badge variant="info" text="virtualenvs.clear"] : Nettoie le paramètre de l'environnement s'il existe déjà<br>
[!badge variant="info" text="virtualenvs.upgradepip"] : Met à jour pip au moment de la création<br>
[!badge variant="info" text="virtualenvs.in-project"] : Stocke l'environnement dans le projet (sinon dans le cache)<br>
[!badge variant="info" text="virtualenvs.symlinks"] : Utilise des liens symboliques au lieu de copier les fichiers<br>
[!badge variant="info" text="virtualenvs.system-site-packages"] : Autorise l'utilisation des site-packages système<br>
[!badge variant="info" text="virtualenvs.foldername"] : Nom du répertoire des environnements<br>
[!badge variant="info" text="virtualenvs.prompt"] : Défini le modèle de prompt qui sera utilisé dans l'environnement<br>
<br>

#### logs
Ces paramètres seront utilisés pour définir le niveau de logs souhaité.

[!badge variant="info" text="logs.display"] : Affiche les logs de l'application<br>
[!badge variant="info" text="logs.full"] : Affiche les logs détaillés<br>
[!badge variant="info" text="logs.date"] : Ajoute la date dans les logs<br>
[!badge variant="info" text="logs.truecolor"] : Affiche les logs en version truecolor<br>
<br>
#### project
Ces paramètres seront utilisés pour délimiter le comportement du projet.

[!badge variant="info" text="project.changelog"] : Alimentation d'un changelog en cas de changement de version<br>
[!badge variant="info" text="project.deep_search"] : Niveau de recherche pour déterminer si on se trouve dans un projet<br>
<br>

#### publish
Ces paramètres seront utilisés pour publier des packages sur un repo.

[!badge variant="info" text="publish.url"] : URL du repo de package<br>
[!badge variant="info" text="publish.username"] : Nom de l'utilisateur utilisé<br>
<br>
### metadata
Ces paramètres seront utilisés pour définir le comportement lors de la recherche de métadonnées sur un package.

[!badge variant="info" text="metadata.source"] : URL du repo sur lequel chercher les métadonnées<br>

#### repo
Ces paramètres seront utilisés pour définir le comportement du repo de projet.

[!badge variant="info" text="repo.create"] : Initialisation d'un repo en même temps que la création ou l'initialisation d'un projet<br>
[!badge variant="info" text="repo.commit"] : Défini le modèle de message qui sera utilisé pour les commit<br>
[!badge variant="info" text="repo.branch_autocreate"] : Activation du changement de branche automatique en cas de changement de version du projet<br>