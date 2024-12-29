# Projet de Python pour la data science 2024 : Analyse prédictive des emplacements pour stations de recharge électrique à Paris

![borne-elect](https://www.leparisien.fr/resizer/cYsO4FD5plDcQTP0fs25et6cYoM=/932x582/cloudfront-eu-central-1.images.arcpublishing.com/leparisien/6T2RNV7EWBDJHFXYT26MR5NZGA.jpg)

Dans ce projet, nous nous intéressons au réseau de __bornes de recharge de véhicules électriques à Paris__.

Nous disposons d'un jeu de données tiré de plusieurs API publiques de la ville de Paris, obtenu sur la plateforme Challenge Data, gérée par le data lab de l'ENS Paris : https://challengedata.ens.fr/challenges/57. Il recense des informations sur les stations présentes dans le réseau en 2020 et leurs informations de disponibilité en temps réel. Nous avons également importé les données de comptage routier de l'année 2020 à Paris, également disponible publiquement dans les OpenData de la ville de Paris.

L'objectif est de __créer une heuristique__ indiquant s'il faut implanter une ou plusieurs nouvelles stations dans une zone donnée, selon l'état de la disponibilité des stations et le trafic dans la zone. Nous verrons dans quelle mesure le trafic est une variable pouvant justifier l'implantation de nouvelles stations. Le déroulé du projet est contenu dans le notebook main.ipynb.

Enfin nous proposerons une approche différente, inspirée d'un projet similaire mené sur le réseaux des bornes de recharge en Allemagne : https://github.com/akansh12/data-science-Optimal-EV-station-placement. Celle-ci s'appuie sur des librairies de Open Street Map pour étudier la répartition des bornes de recharge selon la proximité avec des lieux publics : écoles, restaurants, espaces verts, etc. Voir les notebooks __Evolution.ipynb__, __Data_collection_Open_Street_Map.ipynb__ et __Prediction_with_OSM_data.ipynb__.

Description des notebooks
- __main.ipynb__ : notebook principal.
- __import_trafic.ipynb__: conversion des données de comptage routier du format .txt à .csv pour la semaine d'étude.
- __transfo_data.ipynb__ : agrégation des variables d'intérêt par carré et par différentes pondérations des valeurs moyennes.
- __cartes_statiques.ipynb__ : carte m2 : distance de la station la plus proche ; et m3 : score (heuristique) par zone.
__cartes_dynamiques.ipynb__ : carte1 : évolution du taux d'occupation moyen par carré en mesurant avec 1 voisin au cours de la semaine ;
carte2 : avec 2 voisins ;
carte3 : taux de congestion moyen du trafic ($k$) par zone au cours de la semaine d'étude.
_Attention à enlever les commentaires pour l'exécution !_

- __Evolution.ipynb__ : prédiction de l'évolution du nombre de stations avec la méthode Prophet
- __Data_collection_Open_Street_Map.ipynb__ : collecte des données via Open Street Map
- __Prediction_with_OSM_data.ipynb__ : prédiction des lieux d'intérêt pour implanter des stations.




