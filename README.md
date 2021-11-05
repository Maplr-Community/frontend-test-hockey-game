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
- [Datas](#datas)
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

## Datas

Nous vous fournirons un jeux de données disponible à la racine du projet au format JSON (`data.json`)

## Soumettre le test

Une fois terminé, veuillez créer un nouveau dépot sur GitHub et l'envoyer par courriel.

**Bonne chance et bon game ! 🏒**
