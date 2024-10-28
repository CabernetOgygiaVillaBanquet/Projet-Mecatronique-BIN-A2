# Projet-Mecatronique-BIN-A2

Base roulante pour robot de cartographie de zone de stockage de
produits radioactifs.

Système à étudier : base roulante autonome à évitement d’obstacles Système complet :
Dans le but de cartographier la radioactivité au sol dans des zones de stockage (entrepôt ou container),
Il faudra réaliser un robot autonome avec 2 roues en propulsion, prévu pour évoluer sur une surface
horizontale (pente < 0.5%) à coefficient d’adhérence variable (zone de stockage donc possibilité de liquides
divers au sol).

Stratégie de cartographie :
Zone à cartographier rectangulaire.
Le robot fait des lignes droites parallèles pour décrire la surface rectangulaire qu’il est censé cartographier.
En cas de rencontre d’un obstacle, il le contourne et reprend sa trajectoire.

La température du milieu de travail du robot peut varier de 0° C à 95 °C et son utilisation est prévue sous 1
1 atm (atmosphère ).
Détection d’obstacle à ultra-sons par 2 capteurs HC SR04 permettant de couvrir 30° de chaque côté de la
ligne de progression du robot.

La base doit :
1. Avancer en ligne droite Il faut donc que les moteurs soient asservis à la même vitesse, sinon une roue
tournera plus vite que l’autre. D’autant que le pont en H ne peut pas délivrer exactement la même puissance
sur les sorties des 2 moteurs.

Nb : pensez également qu’il peut y avoir des liquides plus ou moins visqueux au sol, susceptible de faire
tourner les roues à des vitesses différentes pendant un temps t, c’est là que le choix de votre correction sera
judicieux.

Nb bis : chaque moteur est unique, donc chaque correction aussi.

2. Détecter tout obstacle et le contourner
3. Identifier un mur et faire demi-tour pour parcourir la ligne parallèle suivante

Dans la Version 0 il n’y aura pas de gyroscope embarqué.
On ne tient pas compte du capteur de radioactivité dans la réalisation. Ils sont souvouvent gros et lourds et
dans la Version 0 on veut surtout vérifier la faisabilité des 3 points signalés ci-dessus.
