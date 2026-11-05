# Votre site portable.md

Généré avec [l’éditeur portable.md](https://editor.portable.md/). Plus d’informations : [portable.md](https://portable.md/).

Cette branche contient un site web statique généré par l’éditeur à partir du projet de `main` : aucune étape de compilation et aucun logiciel serveur.

## Contenu de cette branche

- `index.html`, `pages/`, `pmd-reader-dist/` et les fichiers voisins : le site généré et le lecteur qui l’affiche. Ne les modifiez pas : chaque publication les reconstruit.
- `pmd.json`, `portable.md`, `style.css` et `assets/` : une copie de votre projet, que le lecteur charge. Pour continuer à travailler, ouvrez le projet de `main` dans l’éditeur : l’enregistrer met cette branche à jour.
- `.pmd-publish.json` et `.nojekyll` : suivi pour l’éditeur et pour GitHub Pages. Conservez-les.

## Activer GitHub Pages

1. Dans le dépôt, ouvrez **Settings > Pages**. Sous **Build and deployment**, choisissez **Deploy from a branch**, sélectionnez `gh-pages` et `/ (root)`, puis enregistrez.
2. Après une ou deux minutes, le site est en ligne à l’adresse `https://<votre-nom>.github.io/<depot>/`.
3. Dans l’éditeur, ouvrez **Configuration du projet**, renseignez **URL du site (canonique)** avec cette adresse et enregistrez de nouveau, afin que les liens, le plan du site et les aperçus de partage l’utilisent.

## Publier de nouveau

Publiez de nouveau depuis l’éditeur pour mettre à jour le site. Il ne remplace que les fichiers qu’il a créés (ils figurent dans `.pmd-publish.json`) et laisse tout le reste intact.

L’éditeur a écrit ce fichier une seule fois, à la première publication ici. Vous pouvez le modifier ou le supprimer : il ne sera ni touché ni recréé.
