# principes-mathématique-de-premier-cycle
## Contribuer
Lorsque vous contribuez, vous pouvez ajouter votre nom ou pseudo de choix a ```\author{}``` en utilisant le format suivant:

```tex
\author{Author 1\\
Author 2\\
...
}
```

Chaque ```\part``` a son propre fichier contenant les documents LaTeX qui conrespondent aux $\chapter$ qui se font importer dans ```principes-mathematique-de-premier-cycle.tex``` utilisant

```tex
\input{part-name/chapter-name}
```

Par exemple pour la partie d'algèbre linéaire. 

```
.
├── algebra
│   ├── alg-lin.tex
├── principes-mathematique-de-premier-cycle.tex
└── README.md
```

Dans le document LaTeX:

```tex
\part{Algèbre}
\label{...}
\chapter{Algèbre Linéaire}
\label{...}
\input{algebra/alg-lin.tex}
```

### Format des label
Les label usilisent le format ```\label{category:part_name:chap_name:sec_name:name}```. Par exemple pour un lemme sur les racines complexes d'un polynome iréductible dans le chapitre d'algébre linéaire:

```tex
\label{lm:alg:lin:ireduct:complex-roots}
```
