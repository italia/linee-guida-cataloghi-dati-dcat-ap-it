Esempi
======

esempi d'uso per ``dcatapit:Agent``


``JSON-LD``

.. code-block:: json
   :linenos:

        {
          "@id": "http://dati.gov.it/resource/Amministrazione/agid",
          "@type": [
            "foaf:Agent",
            "http://dati.gov.it/onto/dcatapit#\"Agent"
          ],
          "dcterms:identifier": "agid",
          "foaf:name": {
            "@language": "it",
            "@value": "Agenzia per l'Italia Digitale"
          }
        },



``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Amministrazione/agid -->

    <rdf:Description rdf:about="http://dati.gov.it/resource/Amministrazione/agid">
        <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#&quot;Agent"/>
        <rdf:type rdf:resource="&foaf;Agent"/>
        <dct:identifier>agid</dct:identifier>
        <foaf:name xml:lang="it">Agenzia per l'Italia Digitale</foaf:name>
    </rdf:Description>


``RDF/TURTLE``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Amministrazione/agid>
         a               dcatapit:Agent , foaf:Agent ;
         dct:identifier  "agid" ;
         foaf:name       "Agenzia per l'Italia Digitale"
