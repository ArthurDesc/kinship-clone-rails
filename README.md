# Kinship Clone Rails

Ce projet est un clone de [Kinship](https://www.kinshipedu.fr/) développé avec Ruby on Rails 8.0, PostgreSQL et Tailwind CSS.

## 🚀 Démarrage Rapide

### Prérequis
Assurez-vous d'avoir installé tous les prérequis en suivant le guide dans [SETUP.md](SETUP.md).

### Lancer le projet

1. **Démarrer Laragon**
   ```bash
   # Ouvrir Laragon et cliquer sur "Démarrer tout"
   # Vérifier que PostgreSQL est bien démarré (icône verte)
   ```

2. **Installer les dépendances**
   ```bash
   bundle install
   ```

3. **Configurer la base de données**
   ```bash
   rails db:create
   rails db:migrate
   ```

4. **Lancer le serveur**
   ```bash
   # Cette commande lance à la fois le serveur Rails et la compilation Tailwind
   bin/dev
   ```

5. **Accéder à l'application**
   - Ouvrez votre navigateur
   - Visitez [http://localhost:3000](http://localhost:3000)

### Arrêter le serveur
- Utilisez `Ctrl+C` dans le terminal pour arrêter le serveur
- Vous pouvez aussi arrêter tous les services via Laragon

## 📝 Documentation
- [Structure du Projet](docs/STRUCTURE.md)
- [Guide d'Installation](SETUP.md)

## 🛠 Stack Technique
- Ruby 3.2.8
- Rails 8.0.2
- PostgreSQL
- Tailwind CSS
