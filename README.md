# B3 Devops - TP 2
## Info
mail: florian.armenoult@ynov.com
github_username: Floo42

## Présentation

L'objectif du TP est de mettre en place une api en nodeJS associée à un reverse proxy NGINX.
L'API sera reliée à une base de données SQL PostgreSQL et une base Redis.

## Prérequis

La base PostgreSQL étant persistée, il faut activer le partage de fichiers entre la machine hôte et Docker.

## Installation

Après avoir cloner le dépôt : 

Aller a la racine du dépôt et lancer la commande: `docker-compose -f ./docker-compose.dev.yaml up --build`

## Utilisation

`localhost` Page par défaut de NGINX

`localhost/api` Page  de base de l'API, renvoie 'Hello world'

`localhost/api/status` Page de l'API qui affiche le temps écoulé depuis le lancement de la BDD PostgreSQL, ainsi que le nombre de connexions simultanées sur Redis