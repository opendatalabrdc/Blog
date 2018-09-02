# DRAFT
# 2018-09-02 OSM Database Quality Analysis : The Tasking Manager

In[the previous article on this Blog](!Database_Quality_Analysis_Building_overlaps_and_irregular_geometries_Various_cartographic_projects_comparison.md), on August 27, 
 there was an OSM mapping comparison of different cities (sample from cities starting their participation to Open Cities).  

 We continue the comparison with this time a an OSM map sample for August 30 covering the geographical area corresponding to 
 15 OSM mapping tasks completed in recent weeks. 


## «State of the Map» Comparison, Areas recently mapped using the Task Manager

The same two indicators as in the previous article are used for the comparison according to the different Tasks. Warnings are grouped according to
- Warning: Buildings with irregular geometry and invalid polygons
- Error: Overlay of buildings (with other buildings or other objects)

As for the first comparative sample, there is a great variability in the results according to the Tasks. The mapping validation step via the Task Manager does not appear to have a significant impact on the tasks in this sample. Other factors seem more decisive to us.

*Graph 1 - Observation of buildings with irregular forms, Dar Es Salaam*
![Dar Es Salaam](img/Overpass-Dar-Es-Sallaam-Irregular-Geometries.png)

Dans les centres-ville, d'abord, le nombre de bâtiments avec des formes complexes correpond à ce qui est observé sur l'imagerie aérienne et il est donc normal d'y obsrver des taux de formes comples plus élevés que dans d'autres zones géographiques. Au Centre-ville de Dar Es Salaam et d'autres villes de Tanzanie, on observe ces formes irrégulières. Dans la base OSM, elles représentent de 10% jusqu'à 20% selon les tâche. 
In city centres, first, the number of buildings with complex shapes corresponds in general to what is observed on aerial imagery and it is therefore normal to observe higher rates of warnings for irregular forms than in other geographical areas. In downtown Dar Es Salaam and other cities in Tanzania, these irregular shapes are observed. In the OSM database, they represent from 10% to 20% depending on the task. 

*Graph 2 - Inaccurate tracings, Kochi, India*
![Dar Es Salaam](img/Overpass-Kochi-India-Irregular-Forms-Validation.png)

In Kochi - India, we also find more complex architectures but in smaller numbers. In this case, we observe many individual houses that have been trace with imprecision. However the number of buildings reported with irregular form does not exceed 7%.

Task 4975 (Ndorwa County, Uganda) particularly draws our attention with over 16,600 buildings out of 28,000 with irregular shapes (irregular warning rate of 58.6% of buildings), and an error rate (superimposed buildings) of 3.5% compared to all buildings in the area covered by this task.  This task has not been validated and the analysis of the mapping of the area shows a very variable quality.

*Pierre Béland*

*Graph 3 - Very approximative buildings tracing, Ndorwa, Ouganda*
![Ndorwa, Ouganda](img/JOSM-TM-4975-Ndorwa-County-Uganda.png)



*Table 1 : Comparison, Topological analysis Reports in % of buildings in the area, Areas covered by the Task Manager*

|	Task * 	|	Buildings	|	Warning Irreg Forms	|	%	|	Error Overlaps +Invalid Polyg	|	%	|	Total Flags % | Validation |
|	:------------------------------------------	|	--------:	|	------:	|	--------:	|	------:	|	------:	|	------:	| :------------|
|		|		|		|		|		|		|		|		||	4954 Muchinga province, Zambia	|	53,748	|	605	|	1.1%	|	56	|	0.1%	|	1.2%	|	Validated	|
|	4958 Beni, Nord-Kivu DRC	|	71,064	|	648	|	0.9%	|	181	|	0.3%	|	1.2%	|	Validated	|
|	4975 Ndorwa County, Uganda	|	28,393	|	16,648	|	58.6%	|	981	|	3.5%	|	62.1%	|	Not Validated	|
|	4994 Kalabo, Zambia	|	4,506	|	395	|	8.8%	|	38	|	0.8%	|	9.6%	|	Not Validated	|
|	4998 Blue Nile State, Sudan	|	1,148	|	49	|	4.3%	|	55	|	4.8%	|	9.1%	|	Not Validated	|
|	5009 North of Kochi, India	|	15,810	|	324	|	2.0%	|	109	|	0.7%	|	2.7%	|	Validated	|
|	5010 North of Kochi, India	|	90,816	|	6,619	|	7.3%	|	1,531	|	1.7%	|	9.0%	|	Not Validated	|
|	5019 Mungala Refugee settlement, Uganda	|	1,728	|	5	|	0.3%	|	28	|	1.6%	|	1.9%	|	Not Validated	|
|	4976 Dar es Salaam, Tanzania 	|	1,238	|	245	|	19.8%	|	62	|	5.0%	|	24.8%	|	Validated	|
|	4978 Magata Karutonga, Tanzania	|	2,086	|	131	|	6.3%	|	18	|	0.9%	|	7.1%	|	Validated	|
|	4991 Data Zetu, Tanzania	|	28,567	|	392	|	1.4%	|	938	|	3.3%	|	4.7%	|	Not Validated	|
|	5011 Jangwani, Tanzania 	|	2,465	|	280	|	11.4%	|	81	|	3.3%	|	14.6%	|	Validated	|
|	5016 Dar es Salaam, Tanzania 	|	1,201	|	192	|	16.0%	|	28	|	2.3%	|	18.3%	|	Validated	|
|	5021 Upanga Mashariki, Dar es Salaam, Tanzania	|	2,724	|	380	|	14.0%	|	92	|	3.4%	|	17.3%	|	Validated	|
|	5022 Mchikichini, Dar es Salaam, Tanzania	|	6,597	|	659	|	10.0%	|	372	|	5.6%	|	15.6%	|	Validated	|
|		|		|		|		|		|		|		|		|
|	Total	|	312,091	|	27,572	|	8.8%	|	4,570	|	1.5%	|	10.3%	|		|

* Tâches provenant du Gestionnaire de tâches OSM ([Instance hotosm](https://tasks.hotosm.org))

