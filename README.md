# TP UI Component Libraries — projet de secours : Headless (Angular Aria)

IMT Atlantique · 1re année alternance · cours « UI Component Libraries »

## À quoi sert ce dépôt

C'est le projet de départ `tp-ui-libs-angular`, avec **Angular Aria déjà installé et configuré**.

Il sert de **secours** : votre enseignant vous le donne si l'installation de votre bibliothèque bloque encore au bout de 15 minutes. Vous pouvez ainsi passer directement au composant.

## Démarrer

Prérequis : Node.js 26 (version LTS), npm et git.

```bash
git clone https://github.com/Orodan/tp-ui-libs-angular-headless
cd tp-ui-libs-angular-headless
npm install
npm start          # http://localhost:4200
```

## Ce qui a déjà été fait

- `npm install @angular/aria @angular/cdk`
- Rien d'autre : Angular Aria ne fournit aucun style ni thème. Vous importez ses directives dans vos composants, et tout le CSS est à écrire.

Prenez une minute pour regarder ces fichiers : c'est exactement ce que vous auriez dû faire vous-mêmes.

```
├── src/
│   ├── app/
│   │   ├── app.html    ← le contenu de la FAQ, à structurer
│   │   ├── app.scss    ← vos styles
│   │   └── app.ts      ← importez ici les directives Angular Aria utilisées
│   ├── index.html
│   └── styles.scss     ← styles globaux
├── public/assets/      ← images et polices
├── design/             ← maquettes
└── style-guide.md      ← couleurs, polices, tailles
```

## À vous de jouer

Construire l'accordéon FAQ avec Angular Aria, d'après les maquettes de `design/` et les couleurs et polices de `style-guide.md`.

Documentation officielle : <https://angular.dev/guide/aria/overview>

## Ce qui est attendu

**Obligatoire**

- Fidèle à la maquette et responsive.
- Utilisable au clavier : Tab pour circuler, Entrée et Espace pour ouvrir et fermer.
- Le focus est visible sur chaque question.

**Bonus**

- Un seul panneau ouvert à la fois.

### Défis, si vous avez fini

À faire dans l'ordre : chaque défi s'appuie sur le précédent.

1. **Aux couleurs de l'IMT** : appliquez la charte IMT à votre accordéon (bleu IMT `#00B8DE`, bleu foncé `#14223C`, gris `#EDF3F4`, police Arial). Le résultat doit rester accessible.
2. **Une charte modifiable en direct** : ajoutez à la page un panneau pour changer la charte en direct (couleurs, police). Les choix sont conservés au rechargement de la page (`localStorage`).
3. **Exporter les tokens** : un bouton télécharge la charte en cours sous forme de fichier `tokens.css`, réutilisable dans le projet.

## La restitution

3 à 4 minutes par groupe :

1. Démo de votre accordéon.
2. Un test au clavier, en direct.
3. Votre choix : pourquoi cette techno, ou ce que vous auriez choisi.
4. Un avantage et une douleur de votre approche.

Puisque vous êtes passés par ce projet de secours, dites aussi **ce qui a bloqué pendant votre installation** : c'est une information précieuse pour la synthèse.

## Assistants IA

Les fichiers `AGENTS.md` et `CLAUDE.md` viennent de Frontend Mentor. La plupart des assistants IA les lisent automatiquement : ils vous guideront par questions et indices, sans écrire la solution à votre place.

## Crédits

Challenge par [Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-wyfFdeBwBz). Police Work Sans sous licence SIL Open Font License (`public/assets/fonts/OFL.txt`).
