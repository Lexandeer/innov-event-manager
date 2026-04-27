# Image de base Node.js
FROM node:20-alpine

# Dossier de travail dans le conteneur
WORKDIR /app

# Copie les fichiers de dépendances
COPY package*.json ./

# Installe les dépendances
RUN npm install

# Copie le reste du code
COPY . .

# Port exposé
EXPOSE 3000

# Commande de démarrage
CMD ["node", "index.js"]