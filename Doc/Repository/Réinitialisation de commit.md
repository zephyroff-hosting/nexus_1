---
icon: /assets/icons/repo-reinit.svg
order: 989
---
La commande [!badge variant="info" text="reset"] nous permet de revenir à un commit précédent tout en annulant les modifications actuelles.

```console
nxs reset {COMMIT_ID}
```

Il existe alors 3 modes de reset
<br>
#### Options

[!badge variant="info" text="--hard"] Toutes les modifications dans l'index intermédiaire et le répertoire de travail seront réinitialisées <br>
[!badge variant="info" text="--soft"] La référence pointe vers le commit choisi sans toucher à l'index intermédiaire ou au répertoire de travail<br>
[!badge variant="info" text="--mixed"] L'index intermédiaire est réinitialisé et les modifications en attente sont déplacées vers le répertoire de travail