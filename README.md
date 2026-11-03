# Votre site portable.md

Généré avec [l’éditeur portable.md](https://editor.portable.md/). Plus d’informations : [portable.md](https://portable.md/).

Ce dossier est un site web statique prêt à publier : aucune étape de compilation et aucun logiciel serveur.

## Contenu de ce dossier

- `index.html`, `pages/`, `pmd-reader-dist/` et les fichiers voisins : le site généré et le lecteur qui l’affiche. Ne les modifiez pas : chaque publication les reconstruit.
- `pmd.json`, `portable.md`, `style.css` et `assets/` : une copie de votre projet, que le lecteur charge. Pour continuer à travailler, ouvrez le projet dans l’éditeur (son dossier, ou un ZIP du projet), pas cette copie, puis exportez de nouveau.
- `.pmd-publish.json` et `.nojekyll` : suivi pour l’éditeur et pour GitHub Pages. Conservez-les.

## Vérifier d’abord

Ouvrez le dossier avec un serveur web local. Ouvrir `index.html` directement depuis le disque ne fonctionne pas, car le lecteur charge ses fichiers en HTTP.

## Publier avec GitHub Pages

1. Créez un dépôt sur GitHub et envoyez-y le contenu de ce dossier (le glisser-déposer fonctionne dans l’interface web).
2. Dans le dépôt, ouvrez **Settings > Pages**. Sous **Build and deployment**, choisissez **Deploy from a branch**, sélectionnez votre branche et `/ (root)`, puis enregistrez.
3. Après une ou deux minutes, le site est en ligne à l’adresse `https://<votre-nom>.github.io/<depot>/`.
4. Dans l’éditeur, ouvrez **Configuration du projet**, renseignez **URL du site (canonique)** avec cette adresse et exportez de nouveau, afin que les liens, le plan du site et les aperçus de partage l’utilisent.

L’éditeur peut aussi publier directement vers un dépôt GitHub, sans envoi manuel.

## Publier ailleurs

Tout hébergeur de sites statiques convient (Netlify, Cloudflare Pages, votre propre serveur web, etc.). Envoyez le dossier de sorte que `index.html` soit à la racine de l’adresse web, sans commande de compilation, et servez-le en HTTPS. Le lecteur charge ses bibliothèques de mathématiques, de diagrammes, de PDF et de dessins depuis `cdn.jsdelivr.net` : une Content-Security-Policy doit donc autoriser cet hôte. Facultatif : donnez aux fichiers à empreinte de `pmd-reader-dist/` une longue durée de cache, et laissez l’hébergeur compresser le texte.

Vous pouvez supprimer ce fichier : rien n’en dépend.
