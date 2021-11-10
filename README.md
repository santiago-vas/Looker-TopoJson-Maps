# Looker-TopoJson-Maps
A very excplicit way to use map_layer function in looker because any other documentation can explain it better

This will be the result:
visualize in looker maps  ZONES or POLYGONS where can exits differents measures, (age sum as shown in the image)
![image](https://user-images.githubusercontent.com/54046607/141036561-ce29d893-6758-4afc-870a-bcd6b3d88a70.png)


you will need 4 things:

1. A .json file with .topojson format, you can find it as "sur_america_polygons.json" in the repository
2. A looker model where you define the connection to a database that contains the "4th" NECESARY THING, you can find these model as "model_read_map.model" in the repository
3. A looker view where you define a map_layer, dimension and mesaure, you will find it as "view_read_map.view"
4. a database which cointains the measures of the diffrents ZONES or POLYGONS YOU WANT TO PLOT.

IMPORTANT INFORMATION
the only way to relationate the polygons and the database measures is by "property_key" parameter in the map_layer funtcion which you can relate with the "geounit" property in the topojson file, and in the data base connection it has be call the same way. see the images
a) the topojson file view in a json viewr
b) the structure of the database

![image](https://user-images.githubusercontent.com/54046607/141037621-1eb7cfbc-166b-48bd-a1a9-dbb0dd711d32.png)
![image](https://user-images.githubusercontent.com/54046607/141037683-7e903030-1c66-45c7-a3f1-87cdd6afc79d.png)

once you have these important file: the polygons shapes and the information by shapes you use the codes 2 and 3 which are in this repository

obviuosly you can read any documentation related to map_layer in looker community

if you have any doubt don´t hesitate to ask me


