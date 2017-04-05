Elementi obbligatori
====================


Formato Distribuzione ``dct:format``
------------------------------------

================  =====================================================================================================
elemento          valore
================  =====================================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | Il formato della Distribuzione del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Distribuzione (Distribution) <distribuzione.html>`__ a un oggetto
                  | (codominio) di tipo dct:MediaTypeOrExtent
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/format
================  =====================================================================================================


.. note::
    Scegliere il formato in cui è reso disponibile il file relativo alla distribuzione descritta. Nel caso in cui il formato del file è di tipo “nidificato” (i.e., un file compresso, per esempio nomefile.ttl.zip), si raccomanda di indicare il formato originario del file compresso (nel caso dell’esempio, va indicato il formato ttl). **Per specificare il formato si deve necessariamente utilizzare** il `vocabolario controllato definito a livello Europeo sui "File Type". <http://publications.europa.eu/mdr/resource/authority/file-type/skos/filetypes-skos.rdf>`__




Esempi d'uso di ``dct:format``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcterms:format": {
            "@id": "http://publications.europa.eu/resource/authority/file-type/RDF"
          },
          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
     <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
        <rdf:type rdf:resource="&dcat;Distribution"/>
        <dct:format rdf:resource="http://publications.europa.eu/resource/authority/file-type/RDF"/>
        [altri elementi per specificare la distribuzione]
     </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a           dcatapit:Distribution , dcat:Distribution ;
        dct:format  <http://publications.europa.eu/resource/authority/file-type/RDF> ;
        [altri elementi per specificare la distribuzione]



URL di accesso ``dcat:accessURL``
---------------------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | Un URL tramite cui accedere alla Distribuzione del Dataset. La proprietà lega l'oggetto
                  | (dominio) `Distribuzione (Distribution) <distribuzione.html>`__ a
                  | un oggetto (codominio) di tipo rdfs:Resource
			      | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       https://www.w3.org/ns/dcat#accessURL
================  ===============================================================================================


.. note::
    Inserire l’URL di una pagina web tramite cui si possa accedere alla distribuzione. Essa può essere anche una pagina informativa che fornisce le indicazioni su come ottenere il dataset oppure l'URL di endpoint di accesso al dataset (e.g., SPARQL endpoint). Si consiglia di indicare l’indirizzo completo, comprensivo anche di protocollo (es. http://). **Si raccomanda di usare questa proprietà, e NON la proprietà** `URL di download <distribuzione_elementi_opzionali.html#url-di-download-dcat-downloadurl>`__, **quando non è assolutamente una pagina di download o non si è sicuri che lo sia.**



Esempi d'uso di ``dcat:accessURL``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcat:accessURL": {
            "@id": "http://spcdata.digitpa.gov.it:8899/sparql"
          },
          altri elementi per specificare la distribuzione

``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
        <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
            <rdf:type rdf:resource="&dcat;Distribution"/>
            <dcat:accessURL rdf:resource="http://spcdata.digitpa.gov.it:8899/sparql"/>
            [altri elementi per specificare la distribuzione]
       </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a                 dcatapit:Distribution , dcat:Distribution ;
        dcat:accessURL    <http://spcdata.digitpa.gov.it:8899/sparql> ;
        [altri elementi per specificare la distribuzione]



Licenza ``dct:license``
-----------------------

================  ===============================================================================================
elemento          valore
================  ===============================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | La licenza con la quale è resa disponibile, per il riutilizzo, la Distribuzione del Dataset.
                  | La proprietà lega l'oggetto (dominio) `Distribuzione (Distribution) <distribuzione.html>`__
                  | a un oggetto (codominio) di tipo `Licenza <licenza.html>`__
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/license
================  ===============================================================================================


.. note::
    Per un uso pratico del metadato licenza si vedano `gli esempi di uso della licenza <licenza_esempi.html>. **Si raccomanda tuttavia, in presenza di licenze creative commons, di riferirsi a quelle specificate in http://creativecommons.org come negli esempi sotto riportati.**



Esempi d'uso di ``dct:license``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
           "dcterms:license": {
            "@id": "http://creativecommons.org/licenses/by/4.0/"
          },
          altri elementi per specificare la distribuzione


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->
    <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
        <rdf:type rdf:resource="&dcat;Distribution"/>
        <dct:license rdf:resource="http://creativecommons.org/licenses/by/4.0/"/>
        [altri elementi per specificare la distribuzione]
    </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a             dcatapit:Distribution , dcat:Distribution ;
        dct:license   <http://creativecommons.org/licenses/by/4.0/> ;
        [altri elementi per specificare la distribuzione] .
