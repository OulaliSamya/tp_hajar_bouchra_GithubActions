FROM node:18

WORKDIR /app

# Installer les dépendances
COPY package*.json ./
RUN npm install --production

# Copier le code
COPY . .

# Variables d'environnement pour la prod
ENV NODE_ENV=production
ENV PORT=8080

# Port exposé à l'intérieur du conteneur
EXPOSE 8080

# Commande de démarrage
CMD ["node", "server.js"]
