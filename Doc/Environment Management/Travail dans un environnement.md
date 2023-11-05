---
icon: /assets/icons/env-work.svg
order: 992
---
Il existe plusieurs solutions pour travailler dans un environnement virtuel, ouvrir un environnement, ouvrir le prompt Python ou encore exécuter une commande dans l'environnement.

Entrer dans un environnement virtuel Python signifie configurer votre terminal ou votre invite de commande pour utiliser l'installation Python et les dépendances spécifiques à cet environnement virtuel. Cela isole l'environnement virtuel, garantissant que les commandes Python et les exécutions de scripts utilisent les packages installés dans cet environnement spécifique.
<br><br>
## Entrer dans un environnement

Deux méthodes, utiliser la commande **nxs env** sans aucun paramètre ouvrira l'environnement par défaut 

```console
nxs env
```


Pour entrer dans un environnement spécifique, il faudra utiliser l'argument [!badge variant="info" text="--open"]

```console
nxs env --open {ENVNAME}
```
<br><br>
## Ouvrir le prompt Python

La commande shell va permettre d'ouvrir directement le prompt Python de l'environnement virtuel sans passer par la phase d'entrée dans l'environnement.

```console
nxs shell
```

Sans paramètre, la commande va ouvrir l'environnement par défaut
Pour ouvrir un shell d'un environnement spécifique, il faudra utiliser l'argument [!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"]
<br><br>
## Exécuter une commande ou script

Nexus propose d'exécuter une commande directement dans un environnement sans l'ouvrir.

```console
nxs run {COMMAND}
```

Il est également possible d'exécuter un fichier .py

```console
nxs run {FILE}
```
<br><br>
#### Options

Par défaut, la commande utilisera l'environnement par défaut. Pour utiliser un environnement spécifique, il faudra utiliser l'argument [!badge variant="info" text="-e"] ou [!badge variant="info" text="--env"]

Pour faciliter les tests, il est possible de définir des paramètres qui seront utilisés lors de l'exécution par la commande [!badge variant="info" text="--set"]

```console
nxs run --set {ARGUMENT}
```

Ces paramètres seront stockés dans le fichier du projet et seront utilisés au lancement de la commande run


Il est également possible de dissocier les exécutions de test (avec [!badge variant="info" text="--test"]) et de prod (avec [!badge variant="info" text="--prod"]) pour permettre de réaliser différents tests rapidement

```console
nxs run --prod {FILE}
```


Pour contrôler les temps d'exécutions, l'option [!badge variant="info" text="-T"] ou [!badge variant="info" text="--time"] permet d'afficher le temps de la commande ou du script