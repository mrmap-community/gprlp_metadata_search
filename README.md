# gprlp_metadata_search
QGIS plugin for using the GeoPortal.rlp RESTful SearchInterface (https://documents.geoportal.rlp.de/mediawiki/index.php/SearchInterface) to search and load remote data. There is also another similar interface for a simple remote search in registrated CSW. The registrated CSW interfaces are available in json format: https://www.geoportal.rlp.de/mapbender/php/mod_showCswList.php. The plugin allows searching for datasets and it automatically resolves the coupled services for this datasets while using the european - INSPIRE - way of doing this (https://github.com/INSPIRE-MIF/technical-guidelines/blob/2022.1/metadata/metadata-iso19139/metadata-iso19139.adoc). 
# Video - how it works ;-)
![qgis_3 22_metadata_search_plugin](https://user-images.githubusercontent.com/1188234/154994934-aa8abb57-4b8c-47b3-b18c-c0ad3efb07a1.mp4)
# Options
## Search for 
### Published OWS Context Documents
The GeoPortal..lp registry mangages metadata for user-defined context documents (actual extended OGC WMC 1.1.0 documents). This resources can be published to serve a special theme 
### Map layers (WMS)
## Load layers into QGIS Browser
## Switch between federal catalogues
### Hesse
### Rhineland-Palatinate
### Saarland
