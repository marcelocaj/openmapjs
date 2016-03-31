# OpenMapJS 1.0 Beta

1. Introduction
--------------
OpenMapJS is a program which plots RDF (GeoSPARQL compatible) using an OpenLayer-3 map. 

It has been built using AngularJS, so there is no need of an application server. 

2. Download
----------
Download from here: [OpenMapJS-1.0beta-public.zip](https://www.dropbox.com/s/5kkkpe7zmtv3fci/OpenMapJS-1.0beta-public.zip?dl=0)

If you want instant results, you can upload this RDF to your Parliament:
[realGeoSparqlRDF.zip](https://www.dropbox.com/s/1jgen4q5cjp9yj3/realGeoSparqlRDF.zip?dl=0)

3. Configuration
----------------
The file config.json contains the following settings:
- url: Endpoint's URL. It must be an interface which receives SPARQL; 
for example, the default URL in Parliament is: 
http://localhost:8080/parliament/sparql

- maxResults: It is the maximum number of results used in the application. 
In other words, it is the LIMIT field in a SPARQL query.

4. Use 
------
After a correct configuration (config.json), the html file should be working 
with a web interface.

The interface is integrated by a sidebar and the map. In particular, the 
sidebar puts on view all the subclasses of geosparl:Feature stored in the 
endpoint. Furthermore, each item can be enabled/disabled according you want 
to see in the map. In addition, each feature can be clicked to see which 
Latitude/Longitude and label corresponds to that point. 

5. Limits
---------
The map has been tested with Parliament (v2.7.9 and 2.7.10) Endpoint only. 
However, tests were performed with Marmotta+GeoSPARQL-module but they were 
lacking of inference, so future test will be carried out when Marmotta 
includes that characteristic. 

This application is compatible only with GeoSPARQL, any other geographical 
standard is not recognized.

6. Preview
----------
![OpenMapJS](http://i.imgur.com/Xzm7Z3g.png)

7. License
----------
This application is distributed under GNU/LGPL License v3.
