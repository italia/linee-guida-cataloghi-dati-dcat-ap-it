Elementi obbligatori
====================


Nome punto di contatto ``vcard:fn``
---------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       Il nome del contatto stabile per il dataset
Riferimento       http://www.w3.org/2006/vcard/ns#fn
================  ============================================================================================


.. note::
    **E’ fortemente raccomandato indicare il nome di uno specifico ufficio (unità organizzativa) responsabile della raccolta delle richieste/commenti e della predisposizione delle relative risposte**. Solo se non è possibile individuare il riferimento dell’ufficio, si può indicare l’organizzazione nel suo complesso. **Sono da evitare comunque nomi di singole persone**. Questo metadato deve essere specificato qualora si inseriscano informazioni di contatto per il dataset. Per esempio, per il dataset LOD dell’Indice della Pubblica amministrazione il nome dell’ufficio/organizzazione è “banche dati e open data".




Email punto di contatto ``vcard:hasEmail``
------------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | L’indirizzo email del punto di contatto per il Dataset. La proprietà lega l'oggetto
                  | (dominio) `Punto di Contatto <punto-di-contatto.html>`__ a un oggetto (codominio) di tipo vcard:Email
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://www.w3.org/2006/vcard/ns#hasEmail
================  ============================================================================================


.. note::
    **Indicare l’indirizzo email primario dell’ufficio (o gestito dall’ufficio) identificato come punto di contatto per il dataset**. Se non è possibile identificare l’ufficio, si può inserire l’indirizzo email principale dell’organizzazione. **Evitare in ogni caso di specificare indirizzi email di singole persone fisiche**. Questo metadato deve essere specificato qualora si inseriscano informazioni di contatto per il dataset. **Esempio** --> “mailto:info@dati.gov.it"
