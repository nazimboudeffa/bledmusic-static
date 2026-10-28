# Bledmusic

Un hommage à **Bled Music** et à la mémoire musicale algérienne : émissions, artistes, clips et souvenirs partagés.

Le site est une maquette statique en construction. Il propose une première présentation du projet et des exemples de collections à enrichir avec des archives vérifiées.

## Aperçu

- Page d’accueil avec une identité visuelle inspirée des affiches musicales rétro et une sélection de trois fiches.
- Page dédiée aux archives, consultable par catégorie et par recherche.
- Fenêtres de présentation pour les entrées de la collection.
- Section sur le projet et bouton de contribution renvoyant vers le dépôt GitHub.
- Mise en page adaptée aux écrans mobiles.

> Les cartes et vignettes actuelles sont illustratives : elles ne contiennent pas d’archives vidéo originales.

## Lancer le site en local

Aucune installation ni dépendance n’est nécessaire. Vous pouvez ouvrir `index.html` directement dans un navigateur. Pour utiliser un serveur local, lancez à la racine du projet :

```bash
python -m http.server 8000
```

Puis ouvrez [http://localhost:8000](http://localhost:8000).

## Structure

```text
.
├── index.html   # Accueil, styles et interactions JavaScript
├── archives.html # Collection filtrable
└── images/      # Visuels utilisés par les cartes d’archives
```

Le site est volontairement autonome : le HTML, le CSS et le JavaScript de chaque page sont réunis dans son fichier HTML.

## Mettre à jour la collection

Les cartes de la collection se trouvent dans `archives.html`. La page d’accueil affiche les trois premières fiches et renvoie vers cette collection. Pour ajouter ou modifier une entrée :

1. Adaptez le contenu d’une carte `<article class="archive-card">`.
2. Choisissez une catégorie existante (`emission`, `clips` ou `artistes`) dans `data-category`.
3. Mettez à jour `data-search` avec des mots-clés utiles à la recherche.
4. Ajoutez les informations vérifiées, les crédits et, le cas échéant, un lien vidéo autorisé.
5. Vérifiez le rendu sur ordinateur et mobile, ainsi que les filtres et la recherche sur la page des archives.

Les fenêtres de détail sont actuellement des emplacements de présentation. Les liens, dates, crédits et médias réels doivent être vérifiés avant publication.

La fiche « Cheb Fayçal — Sakina » utilise `images/Cheb Fayçal - Sakina (1991).jpg` et propose deux écoutes Spotify : une version ancienne et une nouvelle version du titre.

## Contribuer

Les idées, souvenirs et pistes d’archives sont les bienvenus. Le bouton **« Proposer une archive »** sur le site ouvre une fenêtre avec un lien vers ce dépôt. Vous pouvez également consulter le dépôt et, si vous souhaitez modifier le site, proposer vos changements dans une pull request.

Avant de partager ou de publier une photo, une vidéo ou un témoignage, vérifiez les droits applicables et obtenez le consentement nécessaire. N’ajoutez pas de contenu privé ou dont vous n’êtes pas autorisé à disposer.

## Technologies et vérifications

- HTML, CSS et JavaScript natifs
- Aucun framework, outil de compilation ou paquet à installer
- Vérification manuelle dans un navigateur après modification

## Droits et affiliation

Bledmusic est un site hommage indépendant, non affilié à l’ENTV ni aux détenteurs des droits de l’émission. Les contenus d’archives restent la propriété de leurs ayants droit.

Aucun fichier de licence n’est fourni dans ce dépôt. Cela ne confère pas d’autorisation de réutiliser les contenus tiers, ni de licence open source au code du projet.
