# Setup Guide pour le Projet Rails

## Prérequis


## Étapes d'installation

### 1. Installation de Ruby

1. Téléchargez Ruby+Devkit depuis [RubyInstaller](https://rubyinstaller.org/downloads/)
   - Choisissez la version Ruby 3.2.x (x64) WITH DEVKIT
   - Suivez l'assistant d'installation
   - À la fin de l'installation, laissez cochée l'option "Run 'ridk install'"

2. Dans la fenêtre MSYS2 qui s'ouvre :
   ```bash
   # Tapez '3' pour installer le MSYS2 and MINGW development toolchain
   3
   ```

### 2. Installation des gems Ruby

```bash
# Mettre à jour RubyGems
gem update --system

# Installer Rails
gem install rails

# Installer Bundler
gem install bundler
```

### 3. Installation de Yarn


2. Installez Yarn via npm :
```bash
npm install -g yarn
```

### 4. Configuration de PostgreSQL via Laragon

1. Ouvrez Laragon
3. Laissez Laragon installer PostgreSQL
4. Notez les informations de connexion par défaut :
   - Username: postgres
   - Password: (vide par défaut)
   - Port: 5432

### 5. Vérification de l'installation

Vérifiez que tout est correctement installé :

```bash
# Vérifier les versions
ruby -v        # Devrait afficher Ruby 3.2.x
rails -v       # Devrait afficher Rails 8.0.x
node -v        # Devrait afficher v20.x.x ou plus récent
yarn -v        # Devrait afficher 1.22.x ou plus récent
psql --version # Devrait afficher PostgreSQL 16.x ou plus récent
```

Lancez les serveurs avec : 

```bash
cd /e/Logiciel/Laragon/laragon/www/kinship-clone-rails && ruby bin/dev
```

Ou avec : 

```bash
cd /e/Logiciel/Laragon/laragon/www/kinship-clone-rails && rails server


cd /e/Logiciel/Laragon/laragon/www/kinship-clone-rails && rails tailwindcss:watch
```
