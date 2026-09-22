# Roulette Française — Probabilités

Application web React/Vite permettant de saisir des résultats de roulette et d’observer les fréquences, séries, écarts et une suggestion statistique indicative.

## Prérequis local

- Node.js 18 ou plus récent
- npm ou pnpm

## Installation et lancement local

Avec npm :

```bash
npm install
npm run dev
```

Avec pnpm :

```bash
pnpm install
pnpm dev
```

Ouvrir ensuite l’adresse affichée par Vite, généralement `http://localhost:5173`.

## Vérification et production locale

```bash
npm run check
npm run build
npm run start
```

Le serveur de production utilise ensuite le port indiqué par la variable `PORT`, ou le port 3000 par défaut.

## Fonctionnalités principales

- Saisie manuelle des résultats réels observés, de 0 à 36.
- Fréquences par numéro, séries de couleur et écarts de session.
- Animation de roue et analyse de session.
- Guide « Comment ça marche ? ».
- Visite guidée interactive avec surbrillance des zones principales.
- Mode « Voir une démonstration » qui charge 12 résultats d’exemple.
- Les données restent dans la session du navigateur ; aucune clé API n’est nécessaire.

## Héberger sur Vercel

1. Créer un compte sur [vercel.com](https://vercel.com).
2. Cliquer sur **Add New → Project**.
3. Importer le dossier du projet depuis GitHub, ou utiliser **Upload** si l’option est proposée.
4. Configurer les paramètres suivants :

```text
Framework preset: Vite
Build command: npm run build
Output directory: dist/public
Install command: npm install
```

5. Cliquer sur **Deploy**.

Si Vercel demande le répertoire racine, sélectionner le dossier qui contient `package.json`.

## Héberger sur Netlify

1. Créer un compte sur [netlify.com](https://www.netlify.com).
2. Ouvrir **Add new site → Import an existing project**.
3. Connecter GitHub ou déposer le dossier du projet.
4. Utiliser :

```text
Build command: npm run build
Publish directory: dist/public
```

5. Cliquer sur **Deploy site**.

## Héberger sur Cloudflare Pages

1. Ouvrir [pages.cloudflare.com](https://pages.cloudflare.com).
2. Cliquer sur **Create a project** puis connecter GitHub.
3. Choisir le dépôt du projet.
4. Utiliser :

```text
Framework preset: Vite
Build command: npm run build
Build output directory: dist/public
```

5. Lancer le déploiement.

## Remarque importante

Cette application est un outil d’analyse de session et de visualisation. Elle n’accède pas aux données internes de Bet261 et ne garantit pas le prochain résultat d’une roulette.
