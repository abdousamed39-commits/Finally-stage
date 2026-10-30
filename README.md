# FITS - Application de Gestion de Stock

> Projet de stage 2026 - Développé par Abdousamed

**🚀 Site en ligne : https://abdousamed39-commits.github.io/Mon-stage/**

![Badge Stage](https://img.shields.io/badge/Stage-2026-blue)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222222)

## 📖 Présentation

Application web de gestion de stock réalisée pour le magasin **FITS** dans le cadre de mon stage de 2026.

L'objectif était de remplacer la gestion manuelle par une interface simple, rapide et utilisable sur mobile.

## ✨ Fonctionnalités Réalisées

- [x] **CRUD Produits** : Ajout et suppression avec confirmation
- [x] **Gestion Quantité** : Boutons +/- avec contrôle (pas de quantité négative)
- [x] **Alertes Visuelles** :
    - Stock faible (≤ 5) : classe `stock-low`
    - Rupture (0) : classe `stock-empty` + bouton - désactivé
- [x] **Recherche Intelligente** : Filtrage instantané par nom, insensible aux accents et majuscules grâce à `normalize("NFD")`
- [x] **Persistance** : Sauvegarde automatique dans `localStorage` (`fits-stock`)
- [x] **Responsive** : Utilisable sur téléphone (voir screenshot)

## 🛠️ Compétences Techniques Mobilisées

**Frontend Vanilla - Sans Framework**

- **HTML5** Sémantique (`<table>`, `<form>`, `aria-label`)
- **CSS3** : Flexbox, classes d'état, responsive
- **JavaScript ES6+ (Version 4 finale)** :
    - `DOMContentLoaded` pour sécuriser le chargement
    - **Event Delegation** : Un seul `addEventListener` sur `productRows` au lieu d'un par bouton (performance)
    - `element.closest()` et `dataset` pour un code moderne
    - API `localStorage` avec `JSON.stringify / parse`

C'est une évolution de mon code : V1 avec `querySelector('button')` -> V4 avec architecture propre et maintenable.

## 📂 Structure du projet
