# Banchage terre-chanvre, retour d'expérience

Page web statique présentant la technique d'isolation par banchage terre-chanvre, à partir d'un cas concret : le doublage d'environ 110 m2 de murs anciens sur 6 cm d'épaisseur.

La page couvre la définition du matériau, le comparatif terre crue contre chaux, un schéma du mur en coupe et de face, la technique pas à pas, une galerie et les remerciements.

## Structure

- `index.html` : la page complète (HTML, CSS et JavaScript autonomes, aucune dépendance de build).
- `assets/img/` : photos du chantier en WebP et AVIF (servies via `picture`, avec repli WebP).
- `imgs/` : photos sources d'origine (non servies).
- `mockups/` : explorations de design (8 directions visuelles), conservées en local et non versionnées.
- `robots.txt`, `sitemap.xml` : référencement.
- `.nojekyll` : désactive le traitement Jekyll de GitHub Pages.

## Référencement (SEO et GEO)

La page inclut des balises Open Graph et Twitter, et des données structurées JSON-LD (Article, HowTo, FAQPage) pour les moteurs de recherche et les moteurs génératifs.

Important : l'URL de base est `https://thibault-santonja.github.io/terre-chanvre/`. Si le site est déployé sur un autre domaine (par exemple un domaine personnalisé), remplacer cette URL partout où elle apparaît : `index.html` (canonical, Open Graph, JSON-LD), `robots.txt` et `sitemap.xml`.

## Aperçu local

Depuis la racine du dépôt :

```
python3 -m http.server 8000
```

Puis ouvrir `http://127.0.0.1:8000/`.

## Déploiement sur GitHub Pages

1. Pousser le dépôt sur GitHub.
2. Dans `Settings` puis `Pages`, choisir `Deploy from a branch`.
3. Sélectionner la branche `main` (ou `master`) et le dossier racine `/`.
4. La page sera servie à l'adresse indiquée par GitHub.

## Photos

Les emplacements photo sont des espaces réservés. Pour intégrer les images du chantier, remplacer les blocs `.ph` par des balises `img` (penser au `loading="lazy"` et à un texte alternatif). Crédit photographique : Thibault Santonja Photographie, thibaultsan.com.

## Sources

- Ecopertica, différence chaux-chanvre et terre-chanvre.
- Alterrebati, fiche technique terre-chanvre.
- Conseils Thermiques, comparatif des isolants.
