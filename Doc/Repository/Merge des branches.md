---
icon: /assets/icons/repo-merge.svg
order: 990
---
Sur des projets disposant de plusieurs branches, il est possible de merge plusieurs branches pour assembler les modifications. Pour cela, on peut utiliser la commande [!badge variant="info" text="branch --merge"]

```console
nxs branch --merge {BRANCH_NAME}
```

La branche choisie sera alors merge dans la branche active.
<br>
#### Options

[!badge variant="info" text="-D"] ou [!badge variant="info" text="--dest"] permet de préciser la branche de destination. Cela permet de merge deux branches sans toucher à la branche active.