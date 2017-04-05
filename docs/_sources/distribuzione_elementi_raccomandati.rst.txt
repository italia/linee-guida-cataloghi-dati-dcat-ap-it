Elementi raccomandati
=====================


Descrizione distribuzione ``dct:description``
---------------------------------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
Cardinalità       0..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Raccomandato
Descrizione       La descrizione della Distribuzione del Dataset
Riferimento       http://purl.org/dc/terms/description
================  ============================================================================================


.. note::
    Specificare una descrizione per la distribuzione, con una breve illustrazione delle sue caratteristiche principali. **Evitare di utilizzare un linguaggio ricco di riferimenti normativi**. Utilizzare invece un linguaggio semplice che possa aiutare qualsiasi utente a identificare la distribuzione. Si ricorda che nessun tag HTML è consentito,



Esempi di uso di ``dct:description``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcterms:description": {
            "@language": "it",
            "@value": "Questa è la distribuzione N3 del dataset Linked Open Data relativo ai contratti
                       del Sistema Pubblico di Connettività"
          },
          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
      <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
          <rdf:type rdf:resource="&dcat;Distribution"/>
          <dct:description xml:lang="it">Questa è la distribuzione N3 del dataset Linked Open Data
                                         relativo ai contratti del Sistema Pubblico di Connettività</dct:description>
          [altri elementi per specificare la distribuzione]
      </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a                dcatapit:Distribution , dcat:Distribution ;
        dct:description  "Questa è la distribuzione N3 del dataset Linked Open Data relativo ai
                         contratti del Sistema Pubblico di Connettività"@it ;
        [altri elementi per specificare la distribuzione]
