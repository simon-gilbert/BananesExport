# BananesExport

L'application BananesExport pour fonctionner s'appuie sur un ensemble de composants :
- Un serveur de présentation basé sur PHP
- Un moteur de base de données MySQL

Afin de pouvoir accéder à l'application, les scripts de déploiements vont devoir gérer les scénarios suivants :
- Création d'un package avec les fichiers php présents dans le répertoire app
- Création automatisé du schéma de base de données MySQL (pas d'import à faire)

En plus de ces éléments, l'utilisateur devra également gérer les installations suivantes :
- Installation d'un mécanisme d'exposition du package
- Installation de la base de données MySQL

Idéalement, il faudrait également un mécanisme de mise à jour du contenu PHP et les données de la base devront être persistantes.

Dernier point, les informations de connexion à la base de données seront exposées auprès de l'application PHP à l'aide de variables d'environnements.

L'ensemble de ces éléments devra faire l'objet d'une documentation minimale afin de pouvoir être pris en main.

## Contraintes techniques

* Le déploiement peut se faire indifféremment dans des containers ou dans des machines
* À la fin de l'exercice, la page d'index et d'info doivent être accessibles depuis un navigateur
* La consultation des pages devra se faire via protocole http sans modifications de paramètres du navigateur et sans lancements de commandes externes
