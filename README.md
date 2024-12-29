# Projet de Python pour la data science 2024 : Analyse prédictive des emplacements pour stations de recharge électrique à Paris

Dans ce projet, nous nous intéressons au réseau de bornes de recharge de véhicules électriques à Paris.

Nous disposons d'un jeu de données tiré de plusieurs API publiques de la ville de Paris, obtenu sur la plateforme Challenge Data, gérée par le data lab de l'ENS Paris : https://challengedata.ens.fr/challenges/57. Il recense des informations sur les stations présentes dans le réseau en 2020 et leurs informations de disponibilité en temps réel. Nous avons également importé les données de comptage routier de l'année 2020 à Paris, également disponible publiquement dans les OpenData de la ville de Paris.

L'objectif est de créer une heuristique indiquant s'il faut implanter une ou plusieurs nouvelles stations dans une zone donnée, selon l'état de la disponibilité des stations et le trafic dans la zone. Nous verrons dans quelle mesure le trafic est une variable pouvant justifier l'implantation de nouvelles stations. Le déroulé du projet est contenu dans le notebook `main.ipynb`.

Enfin nous proposerons une approche différente, inspirée d'un projet similaire mené sur le réseaux des bornes de recharge en Allemagne : https://github.com/akansh12/data-science-Optimal-EV-station-placement. Ceci est disponible dans le notebook : ...

Autres notebooks annexes :
`traffictimestamp.ipynb`: création du dataset sur le comptage routier pour la semaine d'étude, en agrégeant les résultats par zone.
...



