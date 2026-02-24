## TP 5: Gestion avancée des salles

## Objectifs:

Développer un système pour rechercher les salles disponibles selon des créneaux horaires.

Implémenter une recherche multi-critères pour filtrer les salles (capacité, étage, bâtiment, équipements).

Ajouter un mécanisme de pagination pour l’affichage des salles.

Consolider les connaissances sur JPA/Hibernate et la gestion des relations entre entités.

## Prérequis:

Java 8 ou supérieur.

Maven installé.

IDE compatible Java (IntelliJ IDEA, Eclipse, NetBeans…).

Connaissances de base en JPA/Hibernate et SQL.

## Structure du projet:

Le projet est organisé selon les couches classiques :

model : entités JPA représentant la base de données (Utilisateur, Salle, Réservation, Équipement).

repository : interfaces et implémentations pour les requêtes avancées et CRUD.

service : logique métier et gestion des transactions.

util : classes utilitaires (ex. pagination).

main : classe principale pour initialiser les données et tester les fonctionnalités.

## Base de données:

Base H2 en mémoire configurée via persistence.xml.

Les tables sont créées automatiquement au démarrage et supprimées à la fermeture.

## Tables créées :

UTILISATEURS – informations des utilisateurs.

SALLES – informations des salles (nom, capacité, description, bâtiment, étage).

RESERVATIONS – réservations des salles par les utilisateurs.

EQUIPEMENTS – équipements disponibles dans les salles.

SALLE_EQUIPEMENT – table de liaison ManyToMany entre salles et équipements.

## Fonctionnalités principales

Recherche de salles disponibles par créneau

Retourne les salles non réservées pour un intervalle de temps donné.

Recherche multi-critères

Filtres possibles : nom, capacité min/max, bâtiment, étage, équipement.

Pagination des résultats

Limite le nombre de salles affichées par page.

Fournit informations sur la page courante, total de pages et navigation précédente/suivante.

Gestion des données

CRUD complet pour les salles.

Gestion automatique des relations bidirectionnelles avec les réservations et équipements.

## Initialisation et tests

Les données de test incluent :

Plusieurs utilisateurs.

Plusieurs salles avec capacités et équipements variés.

Réservations sur différents créneaux.

Les tests permettent de valider :

Disponibilité des salles selon le créneau.

Recherche multi-critères.

Pagination des résultats.


## Resultat d'execution:



![lab5 HIBERNATE sc1](https://github.com/user-attachments/assets/beba65c8-10c3-4862-8312-6d048c6457bc)


![lab5 HIBERNATE sc2](https://github.com/user-attachments/assets/32ed5e7e-7589-48c0-860e-2d3fa6807933)


![lab5 HIBERNATE sc3](https://github.com/user-attachments/assets/e1fb5627-4145-4173-838a-9af80d8ec1eb)


![lab5 HIBERNATE sc4](https://github.com/user-attachments/assets/eb788e9c-531b-4103-b87b-c5cff2dd73e4)


![lab5 HIBERNATE sc5](https://github.com/user-attachments/assets/49a4f404-78f2-40d7-a14a-c629cfd78aa8)


![lab5 HIBERNATE sc6](https://github.com/user-attachments/assets/144112a7-5592-4101-abde-cc4cf4b85fc8)


![lab5 HIBERNATE sc7](https://github.com/user-attachments/assets/f9e128a4-a19d-4093-8d99-7d7f9bcc0c52)


![lab5 HIBERNATE sc8](https://github.com/user-attachments/assets/d7ab1f92-42f6-44b0-be3a-754ce38bbb4a)


![lab5 HIBERNATE sc9](https://github.com/user-attachments/assets/5bab21b5-980b-44c4-81d6-06de83fead01)


![lab5 HIBERNATE sc10](https://github.com/user-attachments/assets/946d008d-027f-4342-9d5b-9e984843d423)


![lab5 HIBERNATE sc11](https://github.com/user-attachments/assets/0bc38c2b-0aac-4250-8c5c-d408696f1d18)


![lab5 HIBERNATE sc12](https://github.com/user-attachments/assets/2fd467fd-fc3d-4acc-a89e-01106843174b)


![lab5 HIBERNATE sc13](https://github.com/user-attachments/assets/db5a91e1-ef3d-421e-8a4e-e31826b59012)


![lab5 HIBERNATE sc14](https://github.com/user-attachments/assets/d8062f64-632a-4c8b-bb3a-f13aae96f39a)


![lab5 HIBERNATE sc15](https://github.com/user-attachments/assets/fc525844-ddcb-402a-afb0-da003cf66ffb)


![lab5 HIBERNATE sc16](https://github.com/user-attachments/assets/3b314c5c-596e-4b9a-aef1-9bcb05c44ffc)


![lab5 HIBERNATE sc17](https://github.com/user-attachments/assets/fcad5f81-d19d-4239-afa1-fab9b056e6b9)


![lab5 HIBERNATE sc18](https://github.com/user-attachments/assets/b7437617-9e3a-41f8-9240-184528fe88a4)


![lab5 HIBERNATE sc19](https://github.com/user-attachments/assets/1c4288a1-8d7f-4053-a43f-0ffca73b44ae)


![lab5 HIBERNATE sc20](https://github.com/user-attachments/assets/149f3e1b-4762-4c7c-8605-9376513f7784)


![lab5 HIBERNATE sc21](https://github.com/user-attachments/assets/07152b04-2fd8-4961-ba9b-578d6006392e)


![lab5 HIBERNATE sc22](https://github.com/user-attachments/assets/97cbbe2c-fa4f-4fea-8cb6-98b5be5d6b12)


![lab5 HIBERNATE sc23](https://github.com/user-attachments/assets/70ea42ed-a123-494e-b15e-3ba037c790da)


![lab5 HIBERNATE sc24](https://github.com/user-attachments/assets/6181a4cd-8102-44c4-85df-60ba5e1f7ff8)


![lab5 HIBERNATE sc25](https://github.com/user-attachments/assets/83b7dad2-770c-46e4-8026-3d8b56cf8ac5)


![lab5 HIBERNATE sc26](https://github.com/user-attachments/assets/89127f88-86ba-434b-9641-43c482a60891)


![lab5 HIBERNATE sc27](https://github.com/user-attachments/assets/c3824d1b-9d60-48f0-b4d4-7e472640eca4)


















































