Esempi
======

Esempi d'uso per ``dcatapit:Catalog``


``JSON-LD``

.. code-block:: json
   :linenos:

    {
          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "dcat:dataset": [
            {
              "@id": "http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid"
            },
            {
              "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid"
            }
          ],
          "dcat:themeTaxonomy": {
            "@id": "http://publications.europa.eu/resource/authority/data-theme"
          },
          "dcterms:description": {
            "@language": "it",
            "@value": "Il catalogo dei dati aperti della pubblica amministrazione italiana"
          },
          "dcterms:issued": {
            "@type": "xsd:date",
            "@value": "2012-01-15"
          },
          "dcterms:language": {
            "@id": "http://publications.europa.eu/resource/authority/language/ITA"
          },
          "dcterms:modified": {
            "@type": "xsd:date",
            "@value": "2016-03-20"
          },
          "dcterms:publisher": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },
          "dcterms:title": {
            "@language": "it",
            "@value": "Catalogo SPCData"
          },
          "foaf:homepage": {
            "@id": "http://spcdata.digitpa.gov.it/index.html"
          }
        },


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->

    <rdf:Description rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
      <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#Catalog"/>
      <rdf:type rdf:resource="&dcat;Catalog"/>
      <dct:modified rdf:datatype="&xsd;date">2016-03-20</dct:modified>
      <dct:issued rdf:datatype="&xsd;date">2012-01-15</dct:issued>
      <dct:title xml:lang="it">Catalogo SPCData</dct:title>
      <dct:description xml:lang="it">Il catalogo dei dati aperti della pubblica amministrazione italiana</dct:description>
      <dct:publisher rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
      <dcat:dataset rdf:resource="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid"/>
      <dcat:dataset rdf:resource="http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid"/>
      <dct:language rdf:resource="http://publications.europa.eu/resource/authority/language/ITA"/>
      <dcat:themeTaxonomy rdf:resource="http://publications.europa.eu/resource/authority/data-theme"/>
      <foaf:homepage rdf:resource="http://spcdata.digitpa.gov.it/index.html"/>
    </rdf:Description>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Catalogp/datigov_agid >
        a                   dcatapit:Catalog , dcat:Catalog ;
        dct:title           "Catalogo Dati.gov.it"@it ;
        dct:description     "Il catalogo dei dati aperti della pubblica amministrazione italiana"@it ;
        dct:modified        "2016-03-20"^^xsd:date ;
        dct:issued          "2012-01-15"^^xsd:date ;
        dct:publisher       <http://dati.gov.it/resource/Amministrazione/agid> ;
        dct:language        <http://publications.europa.eu/resource/authority/language/ITA> ;
        dcat:dataset        <http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid> ;
        dcat:dataset        <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid> ;
        foaf:homepage       <http://spcdata.digitpa.gov.it/index.html> ;
        dcat:themeTaxonomy  <http://publications.europa.eu/resource/authority/data-theme> .
