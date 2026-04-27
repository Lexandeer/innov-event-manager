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
EXPOSE 4200

# Commande de démarrage Angular
CMD ["npx", "ng", "serve", "--host", "0.0.0.0"]