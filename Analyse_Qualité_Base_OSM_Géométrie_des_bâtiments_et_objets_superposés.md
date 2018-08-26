# 2018-08-26 Analyse Qualité Base OSM: Géométrie des bâtiments et objets superposés
 - Comparaison de différents projets 

Dans un [premier article](Analyse_de_la_géométrie_des_bâtiment_pour_une_meilleure_qualité_OpenStreetMap.md)
 sur ce Blog le 8 août, nous avons présenté notre classification de la forme des bâtiments. À titre d'exemple, nous avons examiné les données OSM des bâtiments dans la base OSM, pour la commune de Kisenso à Kinshasa, et mesuré la proportion de bâtiments de forme irrégulière. Les bâtiments de forme irrégulière sont généralement en petit nombre. Des proportions trop élevées suggèrent de regarder de plus près les données et s'assurer de la qualité du tracage des contours de bâtiments.  Dans les milieux urbains denses, le défi est grand pour tracer avec précision le contour des immeubles et les allées entre ces immeubles. La situation se complique également
lorsque les images disponbiles sont sombres ou floues ou encore si différentes images ne sont pas parfaitement alignées. Les mapathons où un grand nombre de débutants participent sont aussi susceptible de causer des problèmes de qualité de la donnée OSM.

Dans de tels projets, le Gestionnaire de tâches OSM est généralement utilisé pour coordonner les contributions simultanées d'un grand nombre de participants et éviter les collisions et conflits d'édition. Ces outils assurent les gestionnaires d'un projet de cartographie de couvrir systématiquement le territoire lors des étapes de cartographie et de validation des données de la zone. Les divers outils Qualité permettent également de repérer des problèmes dans la zone et les corriger. Cependant, on constate souvent qu'après un mapathon, la donnée peut demeurer inchangée pendant des années faute de contributeurs suffisants pour parcourir la zone et corriger les données. 

L'approche que nous proposons est de développer une approche plus quantitative à l'aide de l'analyse topologique. L'identification des bâtiments de forme irrégulière présente une première mesure. Cela permet également de fournir un fichier contenant ces bâtiments pour valider/corriger à l'aide d'éditeurs tels JOSM. Dans ce cas, le greffon ToDO permet de réviser un à un les objets contenus dans le fichier, valider et corriger si nécessaire.

Dans ce deuxième article sur l'analyse topologique, nous ajoutons le repérage des objets superposés (ie. bâtiments, routes, cours d'eau, polygones occupation du sol, etc).

Nous allons également présenter une comparaison de la cartographie de différentes villes faisant partie du projet Open Cities Africa.

# Analyse Qualité - Superposition des Bâtiments et autres objets

# Comparaison, différentes villes du projet Open Cities Africa

## Accra, 2018-08-25, Task 4969, hotosm

* [Accra, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Accra_hotosm_4969_2018_08_25.geojson)
* [Accra, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Accra_hotosm_4969_2018_08_25.geojson)

## Kisenso. 2018-08-16, Tasks 4947, 4953 & 4958, hotosm

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
