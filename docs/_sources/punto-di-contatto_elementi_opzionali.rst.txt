Elementi opzionali
====================


Telefono punto di contatto ``vcard:hasTelephone``
-------------------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       | Il telefono del contatto stabile per il dataset. La proprietà lega l'oggetto
                  | `Punto di Contatto <punto-di-contatto.html>`__ a un oggetto (codominio) di tipo vcard:TelephoneType
                  | (specificato mediante un URI - Uniform Resource Identifier).
Riferimento       http://www.w3.org/2006/vcard/ns#hasTelephone
================  ============================================================================================

.. note::
    **Indicare il numero di telefono dell’ufficio (o gestito dall’ufficio) identificato come punto di contatto per il dataset**. Se non è possibile identificare l’ufficio, si può indicare il numero di telefono del centralino dell’amministrazione. **Evitare in ogni caso di specificare numeri di telefono di singole persone**.



Sito punto di contatto ``vcard:hasURL``
---------------------------------------
================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       | La pagina di contatto per il Dataset. La proprietà lega l'oggetto (dominio)
                  | `Punto di Contatto <punto-di-contatto.html>`__ a un oggetto (codominio) di tipo owl:Thing
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://www.w3.org/2006/vcard/ns#hasURL
================  ============================================================================================


.. note::
    Se esiste, inserire l’URL primario di una pagina di contatto o di un form di contatto. **Evitare il più possibile di indicare l’URL dell’home page dell’organizzazione**. Un esempio di possibile valore per questo metadato è il seguente “http://spcdata.digitpa.gov.it/contattaci.html  (NON dovrebbe essere per esempio “http://www.agid.gov.it”). Nel caso in cui si abbia la necessità di indicare ulteriori URL di interesse per la risorsa descritta, oltre a quello principale, si possono aggiungere più istanze della proprietà foaf:page.
