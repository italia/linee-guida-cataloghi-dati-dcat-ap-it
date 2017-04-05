Esempi
======

Esempi d'uso per ``dcatapit:Distribution``



``JSON-LD``

.. code-block:: json
   :linenos:

     {
          "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"Distribution",
            "dcat:Distribution"
          ],
          "dcat:accessURL": {
            "@id": "http://spcdata.digitpa.gov.it:8899/sparql"
          },
          "dcat:downloadURL": {
            "@id": "http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt"
          },
          "dcterms:description": {
            "@language": "it",
            "@value": "Questa è la distribuzione N3 del dataset Linked Open Data relativo ai contratti del Sistema Pubblico di Connettività"
          },
          "dcterms:format": {
            "@id": "http://publications.europa.eu/resource/authority/file-type/RDF"
          },
          "dcterms:license": {
            "@id": "http://creativecommons.org/licenses/by/4.0/"
          },
          "dcterms:title": "Distribuzione Turtle di LOD SPC Contratti"
     },


``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3 -->

      <dcatapit:Distribution rdf:about="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3">
          <rdf:type rdf:resource="&dcat;Distribution"/>
          <dct:format rdf:resource="http://publications.europa.eu/resource/authority/file-type/RDF"/>
          <dct:title xml:lang="it">Distribuzione Turtle di LOD SPC Contratti</dct:title>
          <dct:description xml:lang="it">Questa è la distribuzione N3 del dataset Linked Open Data relativo ai contratti del Sistema Pubblico di Connettività</dct:description>
          <dct:license rdf:resource="http://creativecommons.org/licenses/by/4.0/"/>
          <dcat:downloadURL rdf:resource="http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt"/>
          <dcat:accessURL rdf:resource="http://spcdata.digitpa.gov.it:8899/sparql"/>
      </dcatapit:Distribution>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3>
        a                 dcatapit:Distribution , dcat:Distribution ;
        dct:title         Distribuzione Turtle di LOD SPC Contratti"@it ;
        dct:description   "Questa è la distribuzione N3 del dataset Linked Open Data relativo ai
                          contratti del Sistema Pubblico di Connettività"@it ;
        dct:format        <http://publications.europa.eu/resource/authority/file-type/RDF> ;
        dct:license       <http://creativecommons.org/licenses/by/4.0/> ;
        dcat:downloadURL  <http://spcdata.digitpa.gov.it/data/contrattiLotto1.nt> ;
        dcat:accessURL    <http://spcdata.digitpa.gov.it:8899/sparql>
