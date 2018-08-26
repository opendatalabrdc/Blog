# 2018-08-26 Analyse Qualité Base OSM: Superpositions et Bâtiments avec Géométrie irrègulière - Comparaison de différents projets
*Figure 1 Polygones non valides / Outils Qualité*
![Figure 1 Polygones non valides](img/Kisenso_test_self_overlap_polygon_vs_osmose_flag.png)

Dans un [premier article](Analyse_de_la_géométrie_des_bâtiment_pour_une_meilleure_qualité_OpenStreetMap.md)
 sur ce Blog le 8 août, nous avons présenté notre classification de la forme des bâtiments. 
À titre d'exemple, nous avons examiné les données OSM des bâtiments dans la base OSM, pour la commune de Kisenso à Kinshasa, et mesuré la proportion de bâtiments de forme irrégulière. Les bâtiments de forme irrégulière sont généralement en petit nombre. Des proportions trop élevées suggèrent de regarder de plus près les données et s'assurer de la qualité du tracage des contours de bâtiments.  Dans les milieux urbains denses, le défi est grand pour tracer avec précision le contour des immeubles et les allées entre ces immeubles. La situation se complique également
lorsque les images disponbiles sont sombres ou floues ou encore si différentes images ne sont pas parfaitement alignées. Les mapathons où un grand nombre de débutants participent sont aussi susceptible de causer des problèmes de qualité de la donnée OSM.

*Figure 2 Polygones non valides - Repérage* ![Figure 2 Polygones non valides - Repérage](img/po-Topologie-FB-Overpass-Kisenso-Polygones-non-valides.png)

Dans de tels projets, le Gestionnaire de tâches OSM est généralement utilisé pour coordonner les contributions simultanées d'un grand nombre de participants et éviter les collisions et conflits d'édition. Ces outils assurent les gestionnaires d'un projet de cartographie de couvrir systématiquement le territoire lors des étapes de cartographie et de validation des données de la zone. Les divers outils Qualité permettent également de repérer des problèmes dans la zone et les corriger. Cependant, on constate souvent qu'après un mapathon, la donnée peut demeurer inchangée pendant des années faute de contributeurs suffisants pour parcourir la zone et corriger les données. 

L'approche que nous proposons est d'extraire les données OSM d'une zone pour une date donnée et réaliser une analyse topologique de la qualité de la donnée.  Les statistiques produites sur les objets signalés pour évaluation permettent de mesurer l'ampleur du phénomène et comparer avec d'autres projets. Cela permet également de fournir un fichier contenant les bâtiments et autres objets à valider/corriger à l'aide d'éditeurs tels JOSM. Dans ce cas, le greffon ToDO permet de réviser un à un les objets contenus dans le fichier, valider et corriger si nécessaire. L'identification des bâtiments de forme irrégulière présentait une première mesure. Les polygones de bâtiments invalides (voir figure 1) ont aussi été identifiés. 

Dans ce deuxième article sur l'analyse topologique, nous ajoutons le repérage des objets superposés (ie. bâtiments, routes, cours d'eau, polygones occupation du sol, etc).

 Lors de la Conférence Open Cities Africa à Dar Es Salaam cette semaine, divers ateliers sont organisés ou les participants des différentes villes faisant partie du porjet Open Cities pourront analyser les données OSM et discuter sur les façons d'améliorer cette donnée.  La comparaison ci-dessous de projets cartographique de différentes villes participantes seront sûrement utiles à la discussion. 
 
# Analyse Qualité - Superposition des Bâtiments et autres objets

Des bâtiments, routes et autres objets tracés avec imprécision ou encore des erreurs lors de l'édition déplaçant un point auront souvent pour effet de superposer des polgyones (bâtiments, occupation du sol, cours d'eau, limites territoriales, etc) et des lignes tels routes et chemins de fer.  La figure 3 illustre ces superpositions, montrant des bâtiments et routes qui se superposent.
sont suSi les bçat

*Figure3 Immeubles et routes superposées*
![Figure 3](img/po-Topologie-XB-XO-Overpass-Kisenso-Vixualise-Immeubles-et-Routes-se-superposant.png)

*Figure 4 Requête Overpass - Id signalés Analyse Qualité*
![Figure 4](img/Overpass_Turbo_Kisenso_Immeubles_formes_irreg.png)

# Comparaison, différentes villes du projet Open Cities Africa

## Accra, 2018-08-25, Task 4969, hotosm

* [Accra, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Accra_hotosm_4969_2018_08_25.geojson)
* [Accra, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Accra_hotosm_4969_2018_08_25.geojson)

## Kisenso. 2018-08-16, (polygone limites de Kisenso)
* [Kisenso, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-kisenso-2018-08-16.geojson)
* [Kisenso, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-kisenso-2018-08-16.geojson)

## Dar Es Salaam, 2018-08-25, Task 5012, hotosm

* [Dar Es Salaam, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_DarEsSalaam_hotosm_5012.geojson)
* [Dar Es Salaam, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_DarEsSalaam_hotosm_5012.geojson)

## Kampala, 2018-04-07, Task 4360, hotosm

* [Kampala, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Kampala_hotosm_4360_2018_04_07.geojson) 
* [Kampala, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Kampala_hotosm_4360_2018_04_07.geojson)

## Monrovia, 2018-08-25, Task 4366, hotosm

* [Monrovia, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_monrovia_hotosm_4866_2018_08_25.geojson) 
* [Monrovia, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-oc_monrovia_hotosm_4866_2018_08_25.geojson)
