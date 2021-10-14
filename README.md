<p align="center">
  <a href="https://github.com/Maplr-Community/nodejs-test-hockey-game">
    <img src="https://maplr.co/wp-content/uploads/2019/12/Fichier-23@3x.png" alt="Logo" height="150">
  </a>
  <h3 align='center'>Test Développeur Frontend intermédiaire</h3>  
  <br />
</p>

## Table des matières

- [Objectif du test](#objectif-du-test)
- [Présomptions](#présomptions)
- [Critères](#critères)
- [Outils à utiliser](#outils-à-utiliser)
- [Modèle](#modèle)
- [API](#api)
  - [GET /api/team/{year}](#GET-/api/team/{year})
  - [POST /api/team/{Year}](#POST-/api/team/{year})
  - [PUT /api/player/captain/{ID}](#PUT-/api/player/captain/{ID})
- [Soumettre le test](#soumettre-le-test)

## Objectif du test

Votre objectif pour ce test est de créer une application web pour ajouter et obtenir les joueurs et les informations de l'équipe de Hockey des Canadiens du Montréal. Le but est donc d'avoir la composition de cette équipe pour chaque année où elle a participé à la Ligue Nationale de hockey.

### **Vous devez créer les fonctionnalités suivantes :**

- Listing des informations de l'équipe et des joueurs en fonction de l'année.
- Possibilité d'ajouter un joueur dans l'équipe d'une année.
- Possibilité de mettre un joueur en capitaine.

## **Présomptions**

- Il n'est pas nécessaire d'implémenter un mécanisme de sécurité.

## Critères

- Les 3 fonctionnalités.
- Qualité du code.
- Utilisation des meilleurs pratiques de développement.

## Outils à utiliser

- Framework JS au choix (react, angular, vues etc...)
- Framework UI au choix (Bootstrap, antd, tailwindcss etc...) (Optionnel)
- Typescript (Optionnel)

## Modèle

Team

```
{
    "id": 1,
    "coach": "Dominique Ducharme"
    "year" : 2020
    "players": [
        {
            "number": 99,
            "name": "John",
            "lastname": "Doe",
            "position": "defenseman",
            "isCaptain" : false
        }
        [...]
    ]
}
```

## API

Nous vous fournissons une api disponible ici : **{api url}**

Vous pouvez utiliser la collection postman incluse dans le projet si vous désirez tester l'API.

Celle-ci se retrouve dans le dossier **postman** du projet.

### GET /api/team/{year}

- Requête: Year dans l'URI
- Réponse: Objet Team (Voir modèle ci-dessus)
- Status: 200 OK

```
http://{api url}/api/team/2020 --header "Content-Type:application/json"

{
    "id": 1,
    "coach": "Dominique Ducharme"
    "year" : 2020
    "players": [
        {
            "number": 99,
            "name": "John",
            "lastname": "Doe",
            "position": "defenseman",
            "isCaptain" : false
        }
        [...]
    ]
}
```

### POST /api/team/{Year}

- Requête: Objet Joueur dans le body
- Réponse: Objet Joueur crée
- Status: 201 CREATED

```
http://{api url}/api/player/2020 --header "Content-Type:application/json"

{
  "number":99,
  "name":"Antonin",
  "lastname":"Bouscarel",
  "position":"forward",
  "isCaptain" : false
}
```

### PUT /api/player/{ID}/captain/

- Requête: ID du joueur dans l'URI
- Réponse: Objet Player
- Status: 200 OK

```
http://{api url}/api/player/9/captain

{
  "number":99,
  "name":"Antonin",
  "lastname":"Bouscarel",
  "position":"forward",
  "isCaptain" : true
}
```

## Soumettre le test

Une fois terminé, veuillez créer un nouveau dépot sur GitHub et l'envoyer par courriel.

**Bonne chance et bon game ! 🏒**
