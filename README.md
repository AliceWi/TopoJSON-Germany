# TopoJSON-Germany
This TopoJSON file of Germany contains its states, counties, important places and furthermore the districts of Berlin in separate objects. 

* counties and Berlin: 
  * id: five digit Community Identification Number
  * properties: name, state, kfz (=license tag), districtType: 
    * Landkreis (=rural district)
    * Kreis (=rural district), only in Schleswig-Holstein and Nordrhein-Westfalen 
    * kreisfreie Stadt (=urban district)
    * Stadtkreis (=urban district), only in Baden-Württemberg    
* states:
  * id: first two digits of the Community Identification Number
  * properties: name, nameEN (=english name, is null if there is none), short (=abbreviation)
* places:
  * id: name
  * properties: name, nameEN (=english name, is null if there is none), state
  

## Note
In the counties the Bodensee is not included.

The shape files I got from [the GADM database](https://www.gadm.org). The districts of Berlin I draw by myself.

Do you want to create your own topoJSON files? These are two usefull tutorials and two great webtools.
* [Command-line-cartography](https://medium.com/@mbostock/command-line-cartography-part-1-897aa8f8ca2c) by Mike Bostok
* [How To Infer Topology](https://bost.ocks.org/mike/topology/) by Mike Bostok
* [Mapshaper](http://mapshaper.org/) by Matthew Bloch
* [geojson.io](http://geojson.io) by Mapbox

By Alice Wittig June 2017
