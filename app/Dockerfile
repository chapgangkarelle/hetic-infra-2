#Utiliser une image de base Node.js officielle
FROM node:16

#Définir le répertoire de travail dans le conteneur
WORKDIR /app

#Copier les fichiers package.json et package-lock.json dans le conteneur
COPY package*.json ./

#Installer les dépendances
RUN npm install

#Copier le reste des fichiers du projet dans le conteneur
COPY . .

#Exposer le port sur lequel l'application tourne
EXPOSE 3000

#Définir la commande pour démarrer l'application
CMD ["node", "app.js"]