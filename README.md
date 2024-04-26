# Fichiers-informatiques-PSCECO05

Ce projet, mené sous la tutelle de Clément Malgouyres (économiste au CREST) a pour objectif d'utiliser le Machine Learning pour optimiser la taxation carbone appliquée aux véhicules en France.

Il s'articule en 3 parties :

Dans un premier temps, cette taxation se base sur le CO2 théorique émis par les véhicules (mesuré en laboratoire). Clément Malgouyres avait observé une grande différence entre ce CO2 théorique et le CO2 réel. Grâce à des méthodes de Machine Learning, Lasso et KNN, il s'agissait dans un premier temps de prédire à l'aide de 25 caractéristiques intrinsèques du véhicule (poids, coefficient d'aérodynamisme, cylindrée...) les émissions de façon beaucoup plus précise pour rendre la taxe plus juste et efficace. On trouvera cette première partie, ainsi que des graphes supplémentaires (courbes d’apprentissage, validation curves) dans le fichier PSC_ML.

Dans un second temps, nous avons étudié l’impact de cette nouvelle modélisation des émissions sur la demande en véhicules neufs, dans la mesure où la taxation, exclusivement dépendante des émissions, s’en retrouve modifiée. On trouvera cette modélisation de la demande, à travers le modèle logit, dans le fichier impact_malus_sur_emissions_AM_reduced.  Ce fichier contient donc également les effets sur les émissions moyennes avec les grilles de taxation 2021 et 2024.

Enfin, dans une troisième partie, nous avons créé une grille de taxation alternative, permettant de diminuer les émissions de manière plus importante. Cette optimisation consiste à maximiser l’utilité globale de tous les consommateurs, sous la contrainte de ne pas dépasser un certain seuil d’émissions. On se réfèrera au fichier p6_optimisation_malus (AM) pour cette dernière partie. On notera que la compilation du fichier p6_optimisation_malus (AM) compile automatiquement le fichier impact_malus_sur_emissions_AM_reduced, qui est nécessité.
