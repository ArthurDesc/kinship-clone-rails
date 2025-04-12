# Accès à la Base de Données PostgreSQL

## 🔑 Informations de Connexion

```
Host: localhost
Port: 5432
Database: kinship_clone_rails_development
Username: postgres
Password: (vide)
```

## 📊 Méthodes d'Accès

### 1. Via pgAdmin 4 (Interface Graphique)

1. Ouvrir Laragon
2. Menu > PostgreSQL > pgAdmin 4
3. Se connecter avec :
   - Email: postgres@localhost
   - Password: (laissez vide)
4. Dans l'arborescence à gauche :
   - Servers > PostgreSQL > Databases > kinship_clone_rails_development

### 2. Via Rails Console

```bash
# Ouvrir la console Rails
rails console

# Exemples d'utilisation
# Lister toutes les tables
ActiveRecord::Base.connection.tables

# Exécuter une requête SQL directe
ActiveRecord::Base.connection.execute("SELECT * FROM users")
```

### 3. Via psql (Ligne de Commande)

1. Ouvrir Laragon
2. Cliquer sur "Terminal"
3. Exécuter :
```bash
psql -U postgres -d kinship_clone_rails_development
```

Commandes psql utiles :
- `\l` : Lister toutes les bases de données
- `\c NOM_BASE` : Se connecter à une base
- `\dt` : Lister les tables
- `\d NOM_TABLE` : Décrire une table
- `\q` : Quitter

### 4. Via le fichier database.yml

Le fichier de configuration de la base de données se trouve dans `config/database.yml`.
Pour modifier les paramètres de connexion, éditez ce fichier. 