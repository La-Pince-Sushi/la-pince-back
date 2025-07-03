# La Pince – Backend

Backend de l’application **La Pince**, projet de fin de formation DWWM. Ce dépôt contient l’API REST développée en **Node.js**, **Express**, et **Sequelize** avec une base de données **PostgreSQL**.

---

## 🚀 Stack technique

- Node.js / Express
- Sequelize ORM
- PostgreSQL
- JavaScript (ES6+)
- Dotenv (environnement de travail défini)
- ESLint
- Joi (validation)
- Cors (gestion des autorisations de requêtes de sources externes)
- Argon2 (hashage mot de passe)

  
---

## 📁 Structure du projet

```bash
la-pince-back/
├── src/
│   ├── database/                # Tout ce qui concerne la base de données
|   ├── docs/                    # Documentation Swagger
│   ├── controllers/             # Gestion des requêtes (handlers)
│   ├── middlewares/             # Middlewares Express (auth, erreurs, etc.)
│   ├── models/                  # Modèles Sequelize
│   ├── router                   # Routes API (Express Router)
|   ├── schemas/                 # Schémas de validation JOI
|   ├── utils/                   # Snippets réutilisables pour améliorer la DX et simplifier les fichiers
│   └── app.js                   # Setup global de l'app (Express, middlewares, routes)
├── .env                         # Variables d'environnement (port, DB)
├── .env.example                 # Modèle de .env pour l'équipe
├── .gitignore
├── package.json
├── README.md
└── server.js                    # Fichier principal qui lance l'app listen
```
---

## ⚙️ Installation

### 1. Cloner le projet

```bash
git clone https://github.com/O-clock-Sushi/la-pince-back.git
cd la-pince-back
```

### 2. Installer les pré-requis d'environnement et dépendances

[Node.js](https://nodejs.org/en/download)

[NPM Version 11.3.0](https://docs.npmjs.com/cli/v11/commands/npm-version)

[Express](https://www.npmjs.com/package/express)

[Dotenv](https://www.npmjs.com/package/dotenv)

[Express XSS Sanitizer](https://www.npmjs.com/package/express-xss-sanitizer)

[Joi](https://www.npmjs.com/package/joi)

[Cors](https://www.npmjs.com/package/cors)

[Argon2](https://www.npmjs.com/package/argon2)

[Sequelize](https://www.npmjs.com/package/sequelize)

[PostgreSQL](https://www.npmjs.com/package/pg)

[Eslint](https://www.npmjs.com/package/eslint)

[JSON Web Token (JWT)](https://www.npmjs.com/package/jsonwebtoken)

```bash
npm install
```
### 3. Configurer l’environnement

Crée un fichier .env à la racine, en te basant sur .env.example :

```env
PORT=3000
DB_NAME=la_pince
DB_USER=postgres
DB_PASSWORD=your_password
DB_HOST=localhost
```

### ▶️ Lancer le projet

En mode développement (avec --watch)
```bash
npm run dev
```
En mode classique
```bash
npm start
```
Le serveur tourne sur http://localhost:3000 (ou le port défini dans .env).

### 🧪 Tests

Tests à venir. Prévu avec Jest et Supertest.

### 📦 Scripts disponibles

Script | Description
npm start | Lance le serveur Express
npm run dev | Lance avec nodemon (rechargement auto)
npm run lint | Lint avec ESLint (à configurer)

### 👥 Équipe projet

Projet réalisé dans le cadre du Titre Professionnel DWWM.

- Scrum Master / Lead Back-End : Baptiste

- Membres de l’équipe à compléter ici

### 📄 Licence

Projet open-source à but pédagogique. Développé pour l’évaluation du titre DWWM.
