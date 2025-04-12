# Structure du Projet

## Organisation MVC

### 📁 Models (`app/models/`)
- Contient la logique métier et les relations entre les modèles
- Gère les validations et les callbacks
- Interagit avec la base de données PostgreSQL

### 📁 Views (`app/views/`)
- Templates ERB avec Tailwind CSS pour le style
- Organisation par contrôleur
- Layouts communs dans `views/layouts/`
- Components réutilisables dans `views/components/`

### 📁 Controllers (`app/controllers/`)
- Gère les requêtes HTTP
- Coordonne l'interaction entre les modèles et les vues
- Implémente la logique de l'application

## Autres Dossiers Importants

### 📁 Assets (`app/assets/`)
- `stylesheets/`: Styles CSS personnalisés
- `images/`: Images et icônes
- `builds/`: Fichiers compilés par Tailwind

### 📁 JavaScript (`app/javascript/`)
- `controllers/`: Contrôleurs Stimulus
- `application.js`: Point d'entrée JavaScript

### 📁 Config (`config/`)
- `routes.rb`: Définition des routes de l'application
- `database.yml`: Configuration de PostgreSQL
- `environments/`: Configurations par environnement

### 📁 DB (`db/`)
- `migrations/`: Modifications de la structure de la base de données
- `schema.rb`: Structure actuelle de la base de données
- `seeds.rb`: Données de test/initiales

### 📁 Tests (`test/`)
- Tests unitaires, d'intégration et système
- Fixtures et mocks pour les tests

## Conventions Rails Importantes

### Nommage
- Models: Singulier, PascalCase (ex: `User`)
- Tables: Pluriel, snake_case (ex: `users`)
- Controllers: Pluriel, PascalCase (ex: `UsersController`)

### Organisation du Code
- DRY (Don't Repeat Yourself)
- Convention over Configuration
- Fat Models, Skinny Controllers

## Workflow de Développement

1. Créer une migration pour les changements de base de données
2. Définir le modèle avec ses relations et validations
3. Créer le contrôleur avec les actions CRUD
4. Implémenter les vues avec Tailwind CSS
5. Ajouter les tests
6. Refactoriser si nécessaire 