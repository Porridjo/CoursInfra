#TODO
FROM node:current-alpine3.18

#COPIE LE CODE SOURCE DANS UN REPERTOIRE QUON CHOISIT
COPY exoplanets /var/www/exoplanets

#ON DOIT MAINTENANT INSTALLER LES DEPENDANCES -> IL FAUT SE POSITIONNER DANS LE REPERTOIRE OU Y A LE PACKAGE.JSON ET FAIRE NPM INSTALL
WORKDIR /var/www/exoplanets

RUN npm install

EXPOSE 3000
CMD [ "node", "app.js" ]