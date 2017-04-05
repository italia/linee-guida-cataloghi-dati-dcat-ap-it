Esempi
======

Esempi d'uso per ``dcatapit:LicenseDocument``


``JSON-LD``

.. code-block:: json
   :linenos:

        {
          "@id": "http://creativecommons.org/licenses/by/4.0/",
          "@type": [
            "http://dati.gov.it/onto/dcatapit#\"LicenseDocument",
            "dcterms:LicenseDocument"
          ],
          "dcterms:type": {
            "@id": "http://purl.org/adms/licencetype/Attribution"
          },
          "foaf:name": "CC BY",
          "owl:versionInfo": "4.0"
        },


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://creativecommons.org/licenses/by/4.0/ -->
     <dcatapit:LicenseDocument rdf:about="http://creativecommons.org/licenses/by/4.0/">
        <rdf:type rdf:resource="&dct;LicenseDocument"/>
        <dct:type rdf:resource="http://purl.org/adms/licencetype/Attribution"/>
        <owl:versionInfo>4.0</owl:versionInfo>
        <foaf:name>CC BY</foaf:name>
     </dcatapit:LicenseDocument>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://creativecommons.org/licenses/by/4.0/>
        a                dcatapit:LicenseDocument , dct:LicenseDocument ;
        dct:type         <http://purl.org/adms/licencetype/Attribution> ;
        foaf:name        "CC BY" ;
        owl:versionInfo  "4.0" .
