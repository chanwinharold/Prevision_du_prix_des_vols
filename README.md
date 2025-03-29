À propos de l'ensemble de données  
INTRODUCTION  
L'objectif de l'étude est d'analyser les données de réservation de vols obtenues sur le site web « Ease My Trip » et de réaliser divers tests d'hypothèses statistiques afin d'en extraire des informations pertinentes. L'algorithme statistique de « régression linéaire » sera utilisé pour entraîner les données et prédire une variable cible continue. « Easemytrip » est une plateforme en ligne de réservation de billets d'avion, et donc une plateforme que les passagers potentiels utilisent pour acheter leurs billets. Une étude approfondie des données permettra de découvrir des informations précieuses, d'une grande valeur pour les passagers.  

Questions de recherche  
L'objectif de notre étude est de répondre aux questions de recherche ci-dessous :  
a) Le prix varie-t-il selon les compagnies aériennes ?  
b) Comment le prix est-il affecté lorsque les billets sont achetés seulement 1 ou 2 jours avant le départ ?  
c) Le prix du billet change-t-il en fonction de l'heure de départ et de l'heure d'arrivée ?  
d) Comment le prix change-t-il en fonction du changement de source et de destination ?  
e) Comment le prix du billet varie-t-il entre la classe économique et la classe affaires ?  

COLLECTE DE DONNÉES ET MÉTHODOLOGIE  
L'outil de scraping Octoparse a été utilisé pour extraire les données du site web. Les données ont été collectées en deux parties : une pour les billets en classe économique et une autre pour les billets en classe affaires. Au total, 300 261 options de réservation de vol distinctes ont été extraites du site. Les données ont été collectées pendant 50 jours, du 11 février au 31 mars 2022.
Les données provenaient de données secondaires et ont été collectées sur le site web Ease my trip.

ENSEMBLE DE DONNÉES  
L'ensemble de données contient des informations sur les options de réservation de vols disponibles sur le site web Easemytrip pour les voyages aériens entre les six principales métropoles indiennes. L'ensemble de données nettoyé contient 300 261 points de données et 11 entités.

CARACTÉRISTIQUES  
Français Les différentes caractéristiques de l'ensemble de données nettoyé sont expliquées ci-dessous :  
1) Compagnie aérienne : Le nom de la compagnie aérienne est stocké dans la colonne compagnie aérienne. Il s'agit d'une caractéristique catégorielle comportant 6 compagnies aériennes différentes.
2) Vol : Le vol stocke les informations concernant le code de vol de l'avion. Il s'agit d'une caractéristique catégorielle.
3) Ville source : Ville d'où décolle le vol. Il s'agit d'une caractéristique catégorielle comportant 6 villes uniques.
4) Heure de départ : Il s'agit d'une caractéristique catégorielle dérivée obtenue en regroupant des périodes de temps en bacs. Elle stocke des informations sur l'heure de départ et comporte 6 étiquettes horaires uniques.
5) Arrêts : Une caractéristique catégorielle avec 3 valeurs distinctes qui stocke le nombre d'escales entre les villes source et de destination.
6) Heure d'arrivée : Il s'agit d'une caractéristique catégorielle dérivée créée en regroupant des intervalles de temps en bacs. Elle comporte six étiquettes horaires distinctes et conserve des informations sur l'heure d'arrivée.
7) Ville de destination : Ville où le vol atterrira. Il s'agit d'une caractéristique catégorielle comportant 6 villes uniques.
8) Classe : Une caractéristique catégorielle qui contient des informations sur la classe des sièges ; il a deux valeurs distinctes : Affaires et Économie.
9) Durée : Une fonctionnalité continue qui affiche le temps total nécessaire pour voyager entre les villes en heures.
10) Jours restants : Il s'agit d'une caractéristique dérivée qui est calculée en soustrayant la date du voyage par la date de réservation.
11) Prix : La variable cible stocke les informations sur le prix du billet.
