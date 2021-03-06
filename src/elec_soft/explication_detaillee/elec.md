# elec

Le [repo elec](https://github.com/ClubRobotInsat/elec) contient le code de la/les carte.s éléctronique.s du club robot.

Le but de la séparation des repos est que le code de chaque carte contienne le minimum de code dupliqué (copier-coller) et que le plus de code commun possible soit dans une librairie dédiée.

Le code de la carte est un peu particulier car nous n'avons pas droit à la librairie standard du langage, seulement à la [libcore](https://docs.rs/rust-libcore/0.0.3/core/).
Il est possible d'ajouter des dépendances si elles peuvent être compilées sans la librairie standard.

Le plus simple pour trouver des librairies est de rechercher les librairies avec le mot clé `no_std` sur [crates.io](https://crates.io/)

Pour compiler le code il suffit de lancer (dans le dossier contenant le fichier `Cargo.toml`:

```
cargo build --release
```

Ou d'utiliser le bouton "build" de l'IDE.
