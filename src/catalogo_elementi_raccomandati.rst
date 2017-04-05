Elementi raccomandati
=====================


Homepage ``foaf:homepage``
--------------------------

================  =======================================================================================
elemento          valore
================  =======================================================================================
Cardinalità       0..1
Stato             Raccomandato
Descrizione       | L'home page del Catalogo. La proprietà lega l'oggetto (dominio)
                  | `Catalog (Catalogo) <catalogo.html>`__ a un oggetto (codominio) di tipo foaf:Document
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://xmlns.com/foaf/0.1/homepage
================  =======================================================================================


 .. note::

    Si raccomanda di indicare l’URL di una pagina web attiva che funge da pagina principale (home page) del catalogo. Si consiglia di indicare l’indirizzo completo, comprensivo anche di protocollo (es. http://). **Esempio** --> "http://spcdata.digitpa.gov.it/index.html".


Esempi d'uso di ``foaf:homepage``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "foaf:homepage": {
            "@id": "http://spcdata.digitpa.gov.it/index.html"
          }

          altri elementi del catalogo


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->

     <rdf:Description rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#Catalog"/>
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <foaf:homepage rdf:resource="http://spcdata.digitpa.gov.it/index.html"/>
        [altri elementi del catalogo]
     </rdf:Description>


``RDF/Turtle``

.. code-block:: json
   :linenos:

    <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a               dcatapit:Catalog , dcat:Catalog ;
        foaf:homepage   <http://spcdata.digitpa.gov.it/index.html>  ;

        [altri elementi del catalogo]



Lingua ``dct:language``
-----------------------

================  ==================================================================================
elemento          valore
================  ==================================================================================
Cardinalità       0..N
Stato             Raccomandato
Descrizione       | La lingua del Catalogo. La proprietà lega l'oggetto
                  | (dominio) `Catalog (Catalogo) <catalogo.html>`__
                  | a un oggetto (codominio) di tipo dct:LinguisticSystem
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/language
================  ==================================================================================



 .. note::

	Indicare una o più lingue utilizzate nel catalogo. La scelta della lingua è regolata dall'uso obbligatorio del `vocabolario definito a livello Europeo sulle lingue <http://publications.europa.eu/mdr/resource/authority/language/skos/languages-skos.rdf>`__.


Esempi d'uso di ``dct:language``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "dcterms:language": {
            "@id": "http://publications.europa.eu/resource/authority/language/ITA"
          },

          altri elementi del catalogo

``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->

     <rdf:Description rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#Catalog"/>
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dct:language rdf:resource="http://publications.europa.eu/resource/authority/language/ITA"/>
        [altri elementi del catalogo]
    </rdf:Description>

``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a             dcatapit:Catalog , dcat:Catalog ;
        dct:language  <http://publications.europa.eu/resource/authority/language/ITA> ;

        [altri elementi del catalogo]


Data di rilascio ``dct:issued``
-------------------------------

================  ==================================================================================
elemento          valore
================  ==================================================================================
Cardinalità       0..1
Stato             Raccomandata
Descrizione       La data di rilascio del Catalogo
Riferimento       http://purl.org/dc/terms/issued
================  ==================================================================================


 .. note::

    E' la data in cui il catalogo è reso disponibile.



Esempi di uso di ``dct:issued``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
            "dcterms:issued": {
            "@type": "xsd:date",
            "@value": "2016-03-20"
          },

          altri elementi del catalogo

``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->
     <dcatapit:Catalog rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dct:issued rdf:datatype="&xsd;date">2016-03-20</dct:issued>
        [altri elementi del catalogo]
     </dcatapit:Catalog>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a          dcatapit:Catalog , dcat:Catalog ;
        dct:issued "2016-03-20"^^xsd:date ;
        [altri elementi del catalogo]



Temi ``dcat:themeTaxonomy``
---------------------------

================  ==================================================================================
elemento          valore
================  ==================================================================================
Cardinalità       0..N
Stato             Raccomandato
Descrizione       | Tema del Catalogo. La proprietà lega l'oggetto (dominio)
                  | `Catalog (Catalogo)<catalogo.html>`__` a un oggetto (codominio)
                  | di tipo skos:Concept (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://www.w3.org/ns/dcat#themeTaxonomy
================  ==================================================================================


 .. note::

    Indicare un sistema di organizzazione della conoscenza (KOS) usato per classificare i dataset del Catalogo. Il valore da utilizzare per questa proprietà è l’URI dei vocabolari utilizzati (**non gli URI dei concetti presenti nel vocabolario**). Nel caso del vocabolario Data Theme, usare questo URI http://publications.europa.eu/resource/authority/data-theme come valore di questa proprietà.



Esempi d'uso di ``dcat:themeTaxonomy``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
            "dcat:themeTaxonomy": {
            "@id": "http://publications.europa.eu/resource/authority/data-theme"
          },

          altri elementi del catalogo


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->
     <dcatapit:Catalog rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dcat:themeTaxonomy rdf:resource="http://publications.europa.eu/resource/authority/data-theme" />
        [altri elementi del catalogo]
     </dcatapit:Catalog>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a                   dcatapit:Catalog , dcat:Catalog ;
        dcat:themeTaxonomy  <http://publications.europa.eu/resource/authority/data-theme> ;
        [altri elementi del catalogo]
