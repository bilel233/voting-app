# Utilisation de l'image de base de Node.js 18
FROM node:18

# Définition du répertoire de travail dans le conteneur
WORKDIR /result

# Copie du contenu du répertoire "result" dans le conteneur
COPY . /result

# Installation des dépendances
RUN npm install

# Commande pour lancer le serveur
CMD ["npm", "start"]