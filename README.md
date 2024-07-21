API-TO-DO-LIST
Description
Ce projet est une application de gestion de tâches avec une architecture full-stack comprenant un frontend React et un backend Node.js/Express. L'application permet aux utilisateurs de s'inscrire, se connecter, et gérer leurs tâches à travers des opérations CRUD (Create, Read, Update, Delete).

Structure du Projet
lua
Copier le code
API-TO-DO-LIST/
│
├── backend/
│   ├── controllers/
│   │   ├── userController.js
│   │   └── taskController.js
│   ├── middlewares/
│   │   └── authenticate.js
│   ├── models/
│   │   ├── index.js
│   │   ├── user.js
│   │   └── task.js
│   ├── routes/
│   │   └── userRoutes.js
│   ├── config/
│   │   └── config.js
│   ├── app.js
│   └── package.json
│
└── frontend/
    ├── public/
    ├── src/
    │   ├── components/
    │   │   ├── Login.js
    │   │   ├── Signup.js
    │   │   ├── TaskList.js
    │   │   ├── TaskDetail.js
    │   ├── App.js
    │   ├── index.js
    ├── package.json
Fonctionnalités
Frontend (React)
Login.js : Composant pour la page de connexion.
Signup.js : Composant pour la page d'inscription.
TaskList.js : Composant pour afficher la liste des tâches.
TaskDetail.js : Composant pour afficher les détails d'une tâche.
Les utilisateurs interagissent avec l'interface utilisateur via ces composants. Les requêtes HTTP (GET, POST, PUT, DELETE) sont envoyées depuis React vers l'API backend pour effectuer des opérations CRUD.

Backend (Node.js/Express)
Routes : Les requêtes HTTP sont reçues par les routes définies dans routes/userRoutes.js.
Contrôleurs : Les routes appellent les fonctions des contrôleurs (userController.js, taskController.js) pour gérer la logique métier.
Modèles : Les contrôleurs utilisent les modèles définis dans Sequelize (models/index.js) pour interagir avec la base de données PostgreSQL.
Middleware : Le middleware d'authentification (middlewares/authenticate.js) vérifie les tokens JWT pour sécuriser les routes.
Base de données (PostgreSQL)
Stocke les informations des utilisateurs et des tâches.
Les modèles Sequelize définis dans models/index.js permettent d'interagir avec la base de données.
Technologies utilisées
Frontend
React : Librairie JavaScript pour construire l'interface utilisateur.
React Router : Pour gérer la navigation entre les différentes pages.
Backend
Node.js : Environnement d'exécution pour JavaScript côté serveur.
Express : Framework web pour créer des serveurs HTTP.
Sequelize : ORM (Object-Relational Mapping) pour interagir avec PostgreSQL.
bcryptjs : Pour hacher les mots de passe.
jsonwebtoken : Pour gérer les tokens JWT pour l'authentification.
body-parser : Middleware pour analyser les corps des requêtes HTTP.
Base de données
PostgreSQL : Système de gestion de base de données relationnelle.
Configuration et Installation
Prérequis
Node.js
PostgreSQL
Installation
Clonez le dépôt :

sh
Copier le code

Backend :

sh
Copier le code
cd API-TO-DO-LIST/backend
npm install
Frontend :

sh
Copier le code
cd ../frontend
npm install
Configuration
Backend : Configurez la base de données PostgreSQL dans backend/config/config.js.

Frontend : Assurez-vous que les requêtes API pointent vers le bon serveur backend.

Démarrage
Démarrez le serveur backend :

sh
Copier le code
cd backend
npm start
Démarrez le serveur frontend :

sh
Copier le code
cd ../frontend
npm start
Utilisation
Accédez à l'interface utilisateur via le navigateur à l'adresse http://localhost:3000.
Inscrivez-vous et connectez-vous pour commencer à gérer vos tâches.
Ressources et Documentation
Diagrammes et UML
Dictionnaires de données
Explication API
Requêtes CRUD
Contribution
Les contributions sont les bienvenues ! Veuillez soumettre une pull request ou ouvrir une issue pour discuter des changements que vous souhaitez apporter.

Licence
Ce projet est sous licence MIT. Voir le fichier LICENSE pour plus de détails.

$ video / ressources explicatives:

Diagrammes et UML : https://www.youtube.com/watch?v=RTRMXxBn0A0&list=PLli0V-hBYkvtQBMw61vTNZBG7u7oxoUVx

Dictionnaires de données: https://www.base-de-donnees.com/dictionnaire-des-donnees/?utm_content=cmp-true

Explication api: https://youtu.be/SC4sEiBje1Q?si=kZsQox77eDFJMHWY


requettes crud :


https://www.youtube.com/watch?v=Rm4__WgPncI&authuser=0

Let's start ! :)




