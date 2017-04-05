Elementi obbligatori della geometria
====================================


I seguenti elementi sono obbligatori se la geometria dell'oggetto spaziale che descrive la copertura geografica del dataset viene specificata.

CRS
---------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | L’indicazione del sistema di riferimento spaziale in cui sono rappresentati i dati.
                  | Secondo quanto indicato in `GeoDCAT-AP <https://joinup.ec.europa.eu/asset/dcat_application_profile/asset_release/geodcat-ap-v10>`__, nelle codifiche GML o WKT
                  | il CRS deve essere specificato come definito in GeoSPARQL
================  ============================================================================================




Coordinate
----------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       Le coordinate dell’area geografica coperta dal Dataset.
================  ============================================================================================



.. note::
    Fornire le coordinate relative alla latitudine e longitudine, espresse nel sistema di riferimento WGS84, del riquadro di delimitazione (bounding box) dell’area geografica coperta dal dataset descritto. Se è stato già indicato un identificativo geografico come URI della classe `Localizzazione <copertura-geografica.html>`__, le coordinate possono essere omesse.



Tipo di geometria
-----------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | Il tipo di geometria che caratterizza l’oggetto spaziale utilizzato per la
                  | localizzazione del Dataset (es., punto (point)).
================  ============================================================================================
