# overpass-turbo
Scratch Pad tests for extracting Open Street Map data


https://overpass-turbo.eu/


[out:json];
area[name="Bernalillo County"]->.searchArea;
(
  node["amenity"="school"](area.searchArea);
  way["amenity"="school"](area.searchArea);
  relation["amenity"="school"](area.searchArea);

  node["amenity"="university"](area.searchArea);
  way["amenity"="university"](area.searchArea);
  relation["amenity"="university"](area.searchArea);
);
out body;
>;
out skel qt;


Node for schools and Univerisities in Bernalillo County, New Mexico


Example exports in repository
