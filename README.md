# Gestion des Auteurs et Livres en PHP (POO)

## Description
Ce projet est un exercice pratique de **Programmation Orientée Objet (POO)** en PHP.  
Il permet de gérer des relations entre auteurs et leurs livres, en mettant en œuvre les concepts fondamentaux de la POO tels que l'encapsulation, les méthodes personnalisées, et l'utilisation de `__toString`.

---

## Fonctionnalités
- Création d'auteurs avec une gestion de leur bibliographie.
- Création de livres associés à un auteur.
- Ajout automatique d’un livre à la bibliographie de l’auteur.
- Affichage de la liste complète des livres d’un auteur.
- Respect des bonnes pratiques de codage : encapsulation, conventions de nommage, et méthodes adaptées.

---

## Installation
1. Clonez ce projet depuis GitHub :
   ```bash
   git clone https://github.com/votre-utilisateur/gestion-auteurs-livres.git
Accédez au répertoire du projet :
bash
Copier le code
cd gestion-auteurs-livres
Assurez-vous que PHP est installé sur votre machine.
Pour vérifier, utilisez la commande :
bash
Copier le code
php --version
Exécutez le fichier principal pour tester le projet :
bash
Copier le code
php index.php
Utilisation
Voici un exemple d'utilisation du projet dans un script PHP :

php
Copier le code
require_once 'Auteur.php';
require_once 'Livre.php';

// Création d'un auteur
$auteur = new Auteur("Victor", "Hugo");

// Création de livres associés à l'auteur
$livre1 = new Livre("Les Misérables", 1862, $auteur);
$livre2 = new Livre("Notre-Dame de Paris", 1831, $auteur);

// Affichage des informations de l'auteur et de sa bibliographie
echo $auteur; // Victor Hugo (Bibliographie : Les Misérables, Notre-Dame de Paris)

// Affichage des informations détaillées d'un livre
echo $livre1; // Les Misérables (1862) écrit par Victor Hugo
Structure des classes
Classe Auteur
Propriétés
nom : Nom de l'auteur.
prenom : Prénom de l'auteur.
bibliographie : Liste des livres écrits par l'auteur.
Méthodes
ajouterLivre(Livre $livre) : Ajoute un livre à la bibliographie de l'auteur.
getBibliographie() : Retourne la liste des livres.
__toString() : Affiche le nom de l'auteur et sa bibliographie.
Classe Livre
Propriétés
titre : Titre du livre.
anneePublication : Année de publication.
auteur : Auteur du livre (relation avec la classe Auteur).
Méthodes
__toString() : Affiche les informations du livre (titre, année, auteur).
Conventions de codage respectées
Encapsulation : Les propriétés des classes sont privées et accessibles via des méthodes (getters et setters).
Conventions PSR-12 : Respect des normes de codage PHP pour une meilleure lisibilité.
Méthodes personnalisées : Les classes sont enrichies avec des méthodes adaptées aux relations entre auteurs et livres.
Améliorations possibles
Implémenter une gestion des erreurs (ex : empêcher la création d’un livre sans auteur).
Ajouter une interface utilisateur (console ou web) pour faciliter la gestion des auteurs et des livres.
Permettre la persistance des données dans une base de données.
Auteur
Ce projet a été réalisé par Votre Prénom et Nom.
N'hésitez pas à ouvrir une issue ou à me contacter pour toute suggestion ou question.

markdown
Copier le code
