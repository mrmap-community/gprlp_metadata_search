# gprlp_metadata_search
QGIS Plugin zur Abfrage der GeoPortal.rlp Metadaten-Suchschnittstelle (https://documents.geoportal.rlp.de/mediawiki/index.php/SearchInterface). Man kann nach registrierten Resourcen suchen und gekoppelte Dienste direkt in den QGIS Browser laden. Neben der Suche im GeoPortal.rlp, kann man auch in den dort registrierten Katalogen suchen. Diese Suche geht über den json-Wrapper der jeweiligen Katalogschnittstelle und löst ebenfalls die Daten-Service Kopplung auf. Die im der jeweiligen GeoPortal.rlp Instanz registrierten Katalogschnittstellen sind als json über folgende URL verfügbar: https://www.geoportal.rlp.de/mapbender/php/mod_showCswList.php. 
Aktuell stehen im Geoportal des Landes Rheinland-Pfalz sowohl der deutsche, als auch der europäische Geodatenkatalog zur Verfügung. **Ein Nutzer hat damit Zugriff auf alle Geodaten der GDI-DE sowie von INSPIRE!** Die Auflösung der Daten-Service Kopplung erfolgt gemäß den Vorgaben der EU INSPIRE-Richtlinie: https://github.com/INSPIRE-MIF/technical-guidelines/blob/2022.1/metadata/metadata-iso19139/metadata-iso19139.adoc#4124-linking-to-provided-data-sets-using-coupled-resource


QGIS plugin for using the GeoPortal.rlp RESTful metadata SearchInterface (https://documents.geoportal.rlp.de/mediawiki/index.php/SearchInterface) to search and load remote data. There is also another similar interface for a simple remote search in registrated CSW. The registrated CSW interfaces are available in json format: https://www.geoportal.rlp.de/mapbender/php/mod_showCswList.php.
**Actually a user get a direct access to the central spatial data catalogue of Germany (Geodatenkatalog.DE) and the european INSPIRE catalogue!** The plugin allows searching for datasets and it automatically resolves the coupled services for this datasets while using the european - INSPIRE - way of doing this (https://github.com/INSPIRE-MIF/technical-guidelines/blob/2022.1/metadata/metadata-iso19139/metadata-iso19139.adoc).

# Video
![qgis_3 22_metadata_search_plugin](https://user-images.githubusercontent.com/1188234/154994934-aa8abb57-4b8c-47b3-b18c-c0ad3efb07a1.mp4)

# Optionen / Options
## Suchressourcen / Search resources
### Datensätze / Datasets
Hier wird nach dem Ressourcentyp "dataset" gesucht. Nach der Selektion eines Datensatztitles in der Trefferliste, werden weitere Metadaten zum Treffer angezeigt. Unter "Weitere Infos" werden die zugehörigen Zugriffsmöglichkeiten über WMS, WFS, ATOM Feeds sowie OGC API Features aufgelistet. Die Selektion einer Zugriffsmöglichkeit zeigt Metadaten zu dieser Option und erlaubt es den Webservice direkt in den QGIS Browser zu übernehmen (WMS / WFS / OGC API Features).

![metadata_search_plugin_dataset_german](https://user-images.githubusercontent.com/1188234/158321601-111e71ca-0b8a-4bea-b0c5-68c52af7efa6.gif)

Search for "dataset". After the selection of the title in the resultlist, some more metadata about the dataset is shown. Under "Further info" the coupled accessoptions via WMS, WFS, ATOM Feed and OGC API Features are shown. The selection of one of this accessoptions give some further metadata about the service and allows to load it directly into QGIS browser (WMS / WFS / OGC API Features).

### Kartenebenen / Map layers
Hier werden alle WMS Layer durchsucht. Ähnlich wie bei der Datensatzsuche erhält man bei Auswahl eines Treffers weitere Metadaten zum jeweiligen Layer und die Möglichkeit ihn direkt in den QGIS Browser zu übernehmen. 

Search for WMS layer. Similar to dataset search, the user gets more metadata about the corresponding layer after its selection. The selected layer can be loaded directly into the QGIS browser.

### Publizierte OWS Context Dokumenten / Published OWS Context Documents
Im GeoPortal.rlp werden auch Metadaten zu Kartenzusammenstellungen in Form von OGC WMC Dokumenten verwaltet. Diese Ressourcen werden können publiziert werden, um einen speziellen thematischen Anwendungsfall abzudecken. Die Kartenzusammenstellungen können auch in Form von OWS Context Dokumenten (https://portal.ogc.org/files/?artifact_id=68826) exportiert werden. Das Plugin kann diese Laden und vorhandene WMS Layer (offerings) in den QGIS Browser zu übernehmen. Weitere Informationen zum OWS Context Standard: http://www.owscontext.org/owc_user_guide/C0_userGuide.html

The GeoPortal.rlp registry mangages metadata for user-defined context documents (actual extended OGC WMC 1.1.0 documents). This resources can be published to serve a special theme. The context documents are also available in form of OWS Context documents (json encoding - https://portal.ogc.org/files/?artifact_id=68826). The plugin can read this documents and allows the loading of defined WMS offerings. Further information about OWS Context: http://www.owscontext.org/owc_user_guide/C0_userGuide.html 

### Entfernte CSW / Remote CSW
Siehe Beschreibung des Plugins zu Begin.

See plugin description at the begin.

#### Geodatenkatalog.DE / German spatial data catalogue
![metadata_search_plugin_remote_csw_german](https://user-images.githubusercontent.com/1188234/158322943-5e01d859-0f68-47f5-8b1a-0eb763f94a1d.gif)
#### INSPIRE Katalog / INSPIRE catalogue
![metadata_search_plugin_remot
e_csw_german_inspire](https://user-images.githubusercontent.com/1188234/158323058-e1b9d8cb-b88d-40e6-abcc-5a48b352081d.gif)

## Wechsel zwischen Länderkatalogen / Switch between federal catalogues
### Rheinland-Pfalz / Rhineland-Palatinate
### Hessen / Hesse
### Saarland / Saarland
