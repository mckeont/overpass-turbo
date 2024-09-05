# overpass-turbo
Scratch Pad tests for extracting Open Street Map data


https://overpass-turbo.eu/

Points
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


MultiPolygons

[out:json];
area[name="Bernalillo County"]->.searchArea;
(
  node["amenity"="school"](area.searchArea);
  way["amenity"="school"](area.searchArea);
  relation["amenity"="school"](area.searchArea);

  node["amenity"="university"](area.searchArea);
  way["amenity"="university"](area.searchArea);
  relation["amenity"="university"](area.searchArea);
  
  node["amenity"="college"](area.searchArea);
  way["amenity"="college"](area.searchArea);
  relation["amenity"="college"](area.searchArea);

  node["amenity"="kindergarten"](area.searchArea);
  way["amenity"="kindergarten"](area.searchArea);
  relation["amenity"="kindergarten"](area.searchArea);
);
out body;
>;
out skel qt;





Example exports in repository
