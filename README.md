# Docker

**Objectifs** : Installation et utilisation de **Docker** 

## Installation de Docker

Installer **Docker Desktop** sur une machine sous le système d'exploitation **Windows** , se référer à la documentation en ligne de **Docker**.

## Dockerisation d'une application Nodejs

Effectuer ce *pas à pas* sur le site web officiel de **Nodejs** :

[Dockerizing a Node.js web app](https://nodejs.org/en/docs/guides/nodejs-docker-webapp/)

Lors de la construction de votre image choisissez la version `node:16-alpine` au lieu de `node:16` dans votre **Dockerfile** , vous aurez ainsi une image plus légère.

Personnaliser le fichier `server.js` , changer le **port** par `3478`, mettre les textes que renvoie le serveur en français.Changer le texte du `Hello World` par un texte de votre choix.

Poster sur votre **fork git** ,le **Dockerfile** dans un répertoire **todo-app**. 

## Docker avec une base de donnée

Effectuer ce *step-by-step* sur le site officiel de **Docker** :

[Docker Get Started](https://docs.docker.com/get-started/)

Faires les étapes :

- Getting Started
- Our application
- Updating our App
- Sharing our App
- Persisting our DB
- Using Docker Compose

Dans la partie **Sharing our App** il faudra créer un compte sur [dockerhub](https://hub.docker.com) et y envoyer votre image **docker**.

Mettre l'url de votre dépôt sur **dockerhub** dans un fichier `url.txt` elle ressemblera à `https://hub.docker.com/u/nom_user_choisit`

Mettre à jour le **docker-compose.yml** avec les versions **LTS** de **nodejs** : `node:16-alpine`

Changer le **port** du **service** `app` sur lequel on va lancer l'application par `8078`

Changer **mysql** par **mariadb** dans le **service** `app` : `MYSQL_HOST: mariadb` 

Changer le **service** `mysql` en `mariadb`

L'image de **mariadb** sera `mariadb:10.6`

Poster sur votre **fork git** ,le **Dockerfile** et le **docker-compose.yml** dans un répertoire **app-nodejs**. 




## Git

- Faite un **fork** du dépôt 
- Travailler dans une branche **develop**
- Faire des **commits atomiques**
- Tous vos **commits** doivent commencer par une majuscule
- Les branches **feature** doivent se nommer **feature/nom_de_la_feature**
- Faites des **pull request**

## Questions

Si vous avez des questions ouvrer des **issues** sur ce dépôt et non sur votre **fork** !.
