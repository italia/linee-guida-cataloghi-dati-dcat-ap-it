Elementi opzionali
==================


Titolo distribuzione ``dct:title``
----------------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Opzionale
Descrizione       Il titolo della Distribuzione del Dataset.
Riferimento       http://purl.org/dc/terms/title
================  ===============================================================================================


.. note::

    Se disponibile o ritenuto opportuno, inserire un titolo della distribuzione. Si raccomanda di non utilizzare acronimi o abbreviazioni incomprensibili. Se si vogliono utilizzare comunque gli acronimi, riportare anche il nome esteso o fornire una loro spiegazione.



Esempi di uso di ``dct:title``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


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


URL di download ``dcat:downloadURL``
------------------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Un URL che rappresenta un link diretto al file scaricabile in un dato formato.
                  | La proprietà lega l'oggetto `Distribuzione (Distribution) <distribuzione.html>`__
                  | a un oggetto (codominio) di tipo rdfs:Resource
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       https://www.w3.org/ns/dcat#downloadURL
================  ===============================================================================================


.. note::
    Indicare l’URL che fornisce il link diretto a un file scaricabile nel formato indicato per la distribuzione. Si consiglia di indicare l’indirizzo completo, comprensivo anche di protocollo (es. http://).



Esempi di uso di ``dcat:downloadURL``


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcat:downloadURL": {
            "@id": "http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt"
          },
          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
    <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
       <rdf:type rdf:resource="&dcat;Distribution"/>
       <dcat:downloadURL rdf:resource="http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt"/>
       [altri elementi per specificare la distribuzione]
    </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a                dcatapit:Distribution , dcat:Distribution ;
        dcat:downloadURL <http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt> ;
        [altri elementi per specificare la distribuzione] .



Ultima modifica distribuzione ``dct:modified``
----------------------------------------------


================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       La data di ultima modifica della Distribuzione del Dataset
Riferimento       http://purl.org/dc/terms/modified
================  ===============================================================================================


.. note::
    Indicare la data di ultima modifica o di aggiornamento della distribuzione.



Esempi d'uso di ``dct:modified``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcterms:modified": {
            "@type": "xsd:date",
            "@value": "2015-05-25"
          },

          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
    <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
        <rdf:type rdf:resource="&dcat;Distribution"/>
        <dct:modified rdf:datatype="&xsd;date">2015-05-25</dct:modified>
        [altri elementi per specificare la distribuzione]
    </dcatapit:Distribution>



``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a               dcatapit:Distribution , dcat:Distribution ;
        dct:modified    "2015-05-25"^^xsd:date ;
        [altri elementi per specificare la distribuzione]




Dimensione in byte ``dcat:byteSize``
------------------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       La dimensione in byte della distribuzione del dataset
Riferimento       https://www.w3.org/ns/dcat#byteSize
================  ===============================================================================================

.. note::
    Indicare il valore della dimensione del file espresso in byte



Esempi d'uso di ``dcat:byteSize``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcat:byteSize": {
            "@type": "xsd:float",
            "@value": "3000"
          },
          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
    <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
       <rdf:type rdf:resource="&dcat;Distribution"/>
       <dcat:byteSize rdf:datatype="&xsd;float">3000</dcat:byteSize>
       [altri elementi per specificare la distribuzione]
    </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a               dcatapit:Distribution , dcat:Distribution ;
        dcat:byteSize   "3000"^^xsd:float ;
        [altri elementi per specificare la distribuzione]
