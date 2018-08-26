# 2018-08-26 OSB Database Quality Analysis : Building overlaps and irregular geometries - Various cartographic projects comparizon

*Figure 1 Invalid Polygons / Quality Tools*
![Figure 1 Invalid Polygons](img/Kisenso_test_self_overlap_polygon_vs_osmose_flag.png)

In a [first article](Bulding_Geometry_Analysis_to_Support_OpenStreetMap_Quality_Analysis.md) on august 8 in this Blog,
, we presented our classification of Building forms. For example, we examined the OSM database buildings data added for the Ebola response in North Kivu, DRC, and measured the proportion of
buildings of irregular shape. These buildings are generally in small numbers. 

A high proportion of buildings with irregular shape in the OSM database for an area is an indication to take a closer look
at the data and validate the quality of the drawing of building contours.  In dense urban environments, there is a great challenge
in accurately tracing building contours and walkways between buildings. The situation is also becoming more complicated
when the aerial imageries available to trace in OSM are dark or blurred or if different images are not perfectly aligned. 
Mapathons where a large number of beginners participate are also likely to cause OSM data quality problems.

*Figure 2 Invalid Polygons Detection* ![Figure 2 Invalid Polygons Detection](img/po-Topologie-FB-Overpass-Kisenso-Polygones-non-valides.png)

In many projects, the OSM Tasking Manager is used to coordinate the simultaneous contributions of a large number of participants and to avoid collisions and edit conflicts. 

These tools ensure that the managers of a mapping project systematically cover the territory during the mapping and data validation stages of the zone. The various Quality tools also make it possible to identify problems in the area and correct them. However, we often find that after a mapathon, the data can remain unchanged for years because there are not enough contributors to go through the area and correct the data. 

The approach we propose is to extract OSM data from an area for a given date and perform a topological analysis of the data quality.  

The statistics produced on the objects flagged for further examination make it possible to measure the extent of the phenomenon and 
make comparizons with other projects. This tool also provides a file containing buildings and other objects to validate/correct 
using editors such as JOSM. In this case, the ToDO plugin allows to revise one by one the objects contained in the file, 
validate and correct if necessary. The identification of buildings of irregular shape was a a first measure. Polygons of invalid buildings (see Figure 1) were also identified. 

In this second article on topological analysis, superimposed objects (ie. buildings, roads, streams, land use polygons, etc) are added to the list of objects flagged for more analysis.

During the Open Cities Africa Conference in Dar Es Salaam this week, the participating cities will discuss the quality of the data. 
This is important to ensure the credibility of volunteered cartographic projects and to provide useful data for different projects that 
require geographic data.   The following comparison of mapping projects from different participating cities and 
the proposed analytical approach will hopefully contribute to this discussion. 

# Quality Analysis - Buildings and other Objects Overlaps



*Figure3 Overlapped Buildings and Roads*
![Figure 3](img/po-Topologie-XB-XO-Overpass-Kisenso-Vixualise-Immeubles-et-Routes-se-superposant.png)


Our topological analysis tool let's identify every building, road, waterway or other object overlapping. A statistic of flagged objects is computed and a ID list of flagged objects is also available. An Overpass query using this ID list (see figure 4) 
let's produce OSM data files containing the objects concerned. This then allows the file to be imported into JOSM for analysis and correction.  The map visualisation from the GeoJSON files presented below for each city, let's have an overview of objects flagged for analysis. It is also possible to zoom in for more detail.

*Figure 4 Overpass Query - Flagged Id's - Quality Analysis*
![Figure 4](img/Overpass_Turbo_Kisenso_Immeubles_formes_irreg.png)

# Comparison, Various towns, project Open Cities Africa

For comparison purposes, we selected cities from the Open Cities Africa project for which OSM tasking manager projects were available.  For the most part, these tasks were 100% mapped and validated.  Each city has its own cartographic history, with rapid response to a disaster or variable quality of imagery, organization of mapathons with beginners, etc. Building architecture from one city to another can also vary and in some cities a higher number of buildings with irregular shapes can really exist.  

During the Ebola outbreak in Monrovia in 2014, the city had to be mapped quickly to help humanitarian teams, despite the poor quality of the imagery available. As the images are still lacking in precision, recent projects have not succeeded in significantly improving quality.  In Kamapala, following a recent mapping project, many duplicates have been added. This topological analysis tool allows you to observe amd reac quickly to make the necessary corrections.

Table 1 presents a comparison of the results obtained with the topological analysis with flagged buildings grouped according to
- Buildings - Irregular geometry and invalid polygons
- Overlapped buildings (with other buildings or other objects)

En moyenne, on observe un taux de signalement de 8,2% des immeubles avec géométrie irrégulière et 3.4% de superpositions  en proportion du total des immeubles. Au total, il y a 11,5% de signalements (objets à valider) en proportion des immeubles. 
On average, a rate of 8.2% of buildings are flagged with irregular geometry and 3.4% with Overlaps, this in proportion of total buildings for the zone. In total, flagged objects (objects to be validated)  represent 11.5% of buildings. 

*Tableau 1 : Topological Analysis Comparison, Flagged objects in % of buildings for the zone, 6 Open Cities Africa projects*

|	Town	|	Buildings	|	Form	|	%	|	Overlaps	|	%	|	Total Flags % |
|	:----------------------------------	|	----------:	|	----------:	|	------:	|	----------:	|	------:	|	----------:	|
|	Kisenso 2018-08-16	|	73609	|	324	|	0.4%	|	391	|	0.5%	|	1.0%	|
|	Kampala 2018-04-07	|	11327	|	1001	|	8.8%	|	343	|	3.0%	|	11.9%	|
|	Ngaoundere 2018-08-06	|	73609	|	9998	|	13.6%	|	4439	|	6.0%	|	19.6%	|
|	Monrovia 2018-08-25	|	4107	|	750	|	18.3%	|	442	|	10.8%	|	29.0%	|
|	Accra 2018-08-25	|	4107	|	1396	|	34.0%	|	17	|	0.4%	|	34.4%	|
|	Dar Es Sallaam 2018-08-25	|	2579	|	334	|	13.0%	|	80	|	3.1%	|	16.1%	|
|	Total Projets analyzed	|	169338	|	13803	|	8.2%	|	5712	|	3.4%	|	11.5%	|


## Kisenso. 2018-08-16, (polygon Kisenso Territory limit)
* [Kisenso, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-kisenso-2018-08-16.geojson)
* [Kisenso, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-kisenso-2018-08-16.geojson)


## Kampala, 2018-04-07, Task 4360, hotosm

* [Kampala, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Kampala_hotosm_4360_2018_04_07.geojson) 
* [Kampala, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Kampala_hotosm_4360_2018_04_07.geojson)



## Ngaoundere, 2018-08-06, Task 4800, hotosm

* [Ngaoundere, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Ngaoundere_hotosm_4800_2018_08_06.geojson) 
* [Ngaoundere, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Ngaoundere_hotosm_4800_2018_08_06.geojson)


## Monrovia, 2018-08-25, Task 4366, hotosm

* [Monrovia, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_monrovia_hotosm_4866_2018_08_25.geojson) 
* [Monrovia, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-oc_monrovia_hotosm_4866_2018_08_25.geojson)


## Accra, 2018-08-25, Task 4969, hotosm

* [Accra, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_Accra_hotosm_4969_2018_08_25.geojson)
* [Accra, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_Accra_hotosm_4969_2018_08_25.geojson)


## Dar Es Salaam, 2018-08-25, Task 5012, hotosm

* [Dar Es Salaam, Irregular Building Forms](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-irregular-forms-OC_DarEsSalaam_hotosm_5012.geojson)
* [Dar Es Salaam, Overlapped objects](https://github.com/opendatalabrdc/Documentation/blob/master/topology/topology-overlap-OC_DarEsSalaam_hotosm_5012.geojson)
