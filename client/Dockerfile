# Utiliser une image Node.js comme base
FROM node:16

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier le fichier package.json et package-lock.json (si disponible)
COPY package*.json ./

# Installer les dépendances de l'application
RUN npm install

# Copier les autres fichiers du projet dans le conteneur
COPY . .

# Exposer le port 3000 (par défaut pour Create React App)
EXPOSE 3000

# Commande pour démarrer l'application
CMD ["npm", "start"]