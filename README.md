# Starter Front WCS - Material UI + Vite + TypeScript

Ce projet est un template de démarrage moderne pour développer des applications React performantes. Il est pré-configuré avec **Material UI**, **Vite**, **TypeScript**, et intègre des outils de qualité de code comme **Biome** et **Husky**.

## 🚀 Fonctionnalités

- **[Vite](https://vitejs.dev/)** : Build tool ultra-rapide pour le développement web moderne.
- **[React](https://react.dev/)** : Bibliothèque JavaScript pour créer des interfaces utilisateurs.
- **[TypeScript](https://www.typescriptlang.org/)** : Superset typé de JavaScript pour un code plus robuste.
- **[Material UI (MUI)](https://mui.com/)** : Bibliothèque de composants React populaire pour un design rapide et esthétique.
- **[Biome](https://biomejs.dev/)** : Toolchain web performante pour le linting et le formatage (remplace ESLint et Prettier).
- **[Husky](https://typicode.github.io/husky/)** : Gestionnaire de hooks Git moderne pour automatiser les tâches (comme le linting avant commit).

## 🛠 Installation

1. Clonez ce dépôt (si ce n'est pas déjà fait) :
   ```bash
   git clone <votre-repo-url>
   cd starter-front-wcs
   ```

2. Installez les dépendances :
   ```bash
   npm install
   ```
   *Note : L'installation initialisera automatiquement Husky via le script `prepare`.*

## 💻 Développement

Pour lancer le serveur de développement local :

```bash
npm run dev
```

L'application sera accessible sur `http://localhost:5173` (ou un autre port si le 5173 est occupé).

## 📜 Scripts Disponibles

Voici la liste des commandes disponibles dans le fichier `package.json` :

| Commande | Description |
| :--- | :--- |
| `npm run dev` | Lance le serveur de développement Vite. |
| `npm run build` | Compile le projet pour la production (TypeScript + Vite). |
| `npm run preview` | Permet de prévisualiser le build de production localement. |
| `npm run lint` | Lance **Biome** pour vérifier la qualité du code et le formatage. |
| `npm run lint:fix` | Lance **Biome** et corrige automatiquement les problèmes (lint & format). |
| `npm run format` | Lance **Biome** pour formater tout le code du projet. |
| `npm run prepare` | Script interne pour installer les hooks Husky. |

## 🛡 Qualité du Code & Git Hooks

### Biome
Nous utilisons **Biome** à la place de la combinaison classique ESLint + Prettier. C'est un outil beaucoup plus rapide qui gère à la fois le formatage et le linter.

- Pour vérifier les erreurs : `npm run lint`
- Pour tout corriger automatiquement : `npm run lint:fix`

### Husky
**Husky** est configuré pour intercepter vos commits.
- **Pre-commit hook** : Avant chaque commit, la commande `npm run lint` est exécutée. Si le code ne respecte pas les standards (erreurs de linter), le commit sera bloqué. Cela garantit que seul du code propre est envoyé sur le dépôt.

## 🤖 Utilisation de l'IA (ChatGPT, Claude, Copilot...)

Ce projet est configuré pour favoriser l'apprentissage. Si vous utilisez des outils d'IA :

- **GitHub Copilot** : Le projet contient des instructions spécifiques pour Copilot afin qu'il agisse comme un mentor plutôt que de donner les réponses.
- **Cursor** : Le fichier `.cursorrules` configure automatiquement l'éditeur pour adopter la même approche pédagogique.
- **ChatGPT / Claude / Autres** : Veuillez copier le contenu du fichier `AI_INSTRUCTIONS.md` au début de votre conversation. Cela demandera à l'IA de vous guider pas à pas sans vous donner la solution finale directement.

## 📂 Structure du Projet

```
starter-front-wcs/
├── .husky/             # Configuration des Git hooks
├── public/             # Fichiers statiques publics
├── src/                # Code source de l'application
│   ├── assets/         # Images, fonts, etc.
│   ├── App.tsx         # Composant racine
│   ├── main.tsx        # Point d'entrée React
│   └── ...
├── biome.json          # Configuration Biome
├── package.json        # Dépendances et scripts
├── tsconfig.json       # Configuration TypeScript
└── vite.config.ts      # Configuration Vite
```
