Elementi opzionali
==================


Titolo dello standard ``dct:title``
---------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Opzionale
Descrizione       Il titolo dello standard.
Riferimento       http://purl.org/dc/terms/title
================  ============================================================================================


.. note::

    Indicare un titolo dello standard comprensibile in quanto il metadato potrebbe essere utilizzato nella ricerca e nelle indicizzazioni (evitare acronimi, evitare codici non esaustivi).  Nel caso di riferimenti normativi, indicare per esempio la tipologia di norma il numero e l’anno e inserire il titolo ufficiale della norma.



Descrizione dello standard ``dct:description``
-----------------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Opzionale
Descrizione       La descrizione dello standard.
Riferimento       http://purl.org/dc/terms/description
================  ============================================================================================


.. note::
    Indicare una descrizione per lo standard. **Evitare di utilizzare un linguaggio ricco di riferimenti normativi**. Utilizzare invece un linguaggio semplice che possa aiutare qualsiasi utente a identificare lo standard riferibile al dataset. Si ricorda che nessun tag HTML è consentito,




Documentazione di riferimento ``dcatapit:referenceDocumentation``
-------------------------------------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | URL attraverso i quali viene fornito l’accesso a documenti di dettaglio
                  | relativi allo Standard indicato.
Riferimento       http://www.dati.gov.it/onto/dcatapit#referenceDocumentation
================  ============================================================================================


.. note::
    Indicare uno o più URL della documentazione di riferimento relativa allo standard. Ad esempio, nel caso della raccomandazione DCAT, alcuni URL relativi alla documentazione di riferimento sono: https://www.w3.org/TR/vocab-dcat/ e https://www.w3.org/ns/dcat.rdf
