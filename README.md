# README
# Mon API

Bienvenue dans le projet **Mon API** ! Ce projet contient une API que j'ai développée pour gérer des ressources utilisateurs. Cette API est construite avec **Ruby on Rails** et permet d'effectuer des opérations **CRUD** (Créer, Lire, Mettre à jour, Supprimer) sur des utilisateurs.

## Table des matières
1. [Prérequis](#prérequis)
2. [Installation](#installation)
3. [Utilisation](#utilisation)
4. [Exemples d'utilisation](#exemples-dutilisation)
5. [Auteurs](#auteurs)

## Prérequis
Avant de pouvoir utiliser l'API, assurez-vous d'avoir les éléments suivants installés sur votre machine :

- **Ruby** : version 2.7 ou supérieure
- **Rails** : version 6.x ou supérieure
- **SQLite3** (ou une autre base de données compatible)
- **npm** (ou **yarn**) pour gérer les dépendances frontend si nécessaire

## Installation

1. Clonez ce repository sur votre machine locale :
    ```bash
    git clone https://github.com/Ahiosp/my-api.git
    ```

2. Accédez au répertoire du projet :
    ```bash
    cd my-api
    ```

3. Installez les dépendances Ruby avec Bundler :
    ```bash
    bundle install
    ```

4. Créez et migrez la base de données :
    ```bash
    rails db:create
    rails db:migrate
    ```

## Utilisation

Une fois l'application installée et la base de données configurée, vous pouvez démarrer l'application avec la commande suivante :

```bash
rails server


## Exemples d'Utilisation
Voici quelques exemples d'appels à l'API :

1. Récupérer toutes les ressources
Endpoint : /api/resources
Méthode : GET
Exemple de réponse :
[
  {
    "id": 1,
    "name": "Resource 1",
    "description": "Description de la ressource 1"
  },
  {
    "id": 2,
    "name": "Resource 2",
    "description": "Description de la ressource 2"
  }
]

2. Créer une ressource
Endpoint : /api/resources
Méthode : POST
Exemple de corps de la requête :
{
  "name": "Nouvelle ressource",
  "description": "Description de la nouvelle ressource"
}

3. Mettre à jour une ressource:
Endpoint : /api/resources/{id}
Méthode : PUT
Exemple de corps de la requête :
{
  "name": "Ressource mise à jour",
  "description": "Nouvelle description"
}

4. Supprimer une ressource
Endpoint : /api/resources/{id}
Méthode : DELETE
Exemple de réponse :
{
  "message": "Ressource supprimée avec succès"
}

## Auteur
Nom de l'auteur : Ahiosp
GitHub : https://github.com/Ahiosp
