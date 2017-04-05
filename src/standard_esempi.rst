Esempi
======

Esempi di uso di ``dcatapit:Standard``


``JSON-LD``

.. code-block:: json
   :linenos:

        {
          "@id": "http://dati.gov.it/resource/Standard/standard-org",
          "@type": [
            "dcterms:Standard",
            "http://dati.gov.it/onto/dcatapit#\"Standard"
          ],
          "dcterms:description": {
            "@language": "en",
            "@value": "The ontology of the organizations"
          },
          "dcterms:title": {
            "@language": "en",
            "@value": "W3C Org organization ontology"
          },
          "http://dati.gov.it/onto/dcatapit#\"referenceDocumentation": [
            {
              "@type": "xsd:anyURI",
              "@value": "https://www.w3.org/TR/vocab-org/"
            },
            {
              "@type": "xsd:anyURI",
              "@value": "https://www.w3.org/ns/org.rdf"
            }
          ]
        },



``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Standard/standard-org -->
    <dcatapit:Standard rdf:about="http://dati.gov.it/resource/Standard/standard-org">
        <rdf:type rdf:resource="&dct;Standard"/>
        <dcatapit:referenceDocumentation rdf:datatype="&xsd;anyURI">https://www.w3.org/TR/vocab-org/</dcatapit:referenceDocumentation>
        <dcatapit:referenceDocumentation rdf:datatype="&xsd;anyURI">https://www.w3.org/ns/org.rdf</dcatapit:referenceDocumentation>
        <dct:title xml:lang="en">W3C Org organization ontology</dct:title>
        <dct:description xml:lang="en">The ontology of the organizations</dct:description>
    </dcatapit:Standard>


``RDF/TURTLE``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Standard/standard-org>
      a                               dcatapit:Standard , dct:Standard ;
      dct:title                       "W3C Org organization ontology"@en ;
      dct:description                 "The ontology of the organizations"@en ;
      dcatapit:referenceDocumentation "https://www.w3.org/ns/org.rdf"^^xsd:anyURI ;
      dcatapit:referenceDocumentation "https://www.w3.org/TR/vocab-org/"^^xsd:anyURI .
