Elementi opzionali
==================


Nome geografico ``locn:geographicName``
---------------------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       Nome proprio associato all'oggetto spaziale.
Riferimento       http://www.w3.org/ns/locn#geographicName"
================  ===============================================================================================


.. note::

    Da indicare solo se non è disponibile un identificativo geografico o non sono note le coordinate.



Geometria ``loc:Geometry``
---------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       La Geometria dell'oggetto spaziale..
Riferimento       http://www.w3.org/ns/locn#Geometry
================  ===============================================================================================

.. note::
    Le proprietà  indicate,  nella  pratica,  possono  essere  specificate  attraverso  diverse  codifiche.  La specifica GeoDCAT-AP prevede che debba essere utilizzata almeno una delle seguenti: GML o WKT.
