Esempi
======

Esempi d'uso per ``dcatapit:Organization``


``JSON-LD``

.. code-block:: json
   :linenos:

       {
         "@id": "http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA",
          "@type": [
            "vcard:Organization",
            "vcard:Kind",
            "http://dati.gov.it/onto/dcatapit#\"Organization"
          ],
          "vcard:fn": "banche dati e open data",
          "vcard:hasEmail": {
            "@id": "mailto:info@dati.gov.it"
          },
          "vcard:hasTelephone": {
            "@id": "_:N423506244f6e46028ea51a957fe407f3"
          },
          "vcard:hasURL": {
            "@id": "http://spcdata.digitpa.gov.it/contattaci.html"
          }
          {
           "@id": "_:N423506244f6e46028ea51a957fe407f3",
           "@type": "vcard:Voice",
           "vcard:value": "06123456"
           },
       },


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA -->
    <dcatapit:Organization rdf:about="http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA">
       <rdf:type rdf:resource="&vcard;Kind"/>
       <rdf:type rdf:resource="&vcard;Organization"/>
       <vcard:hasEmail rdf:resource="mailto:info@dati.gov.it"/>
       <vcard:fn>banche dati e open data</vcard:fn>
       <vcard:hasTelephone rdf:parseType="Resource">
            <vcard:value>06123456</vcard:value>
            <rdf:type rdf:resource="http://www.w3.org/2006/vcard/ns#Voice"/>
       </vcard:hasTelephone>
       <vcard:hasURL rdf:resource="http://spcdata.digitpa.gov.it/contattaci.html"/>
    </dcatapit:Organization>



``RDF/Turtle``

.. code-block:: turtle
   :linenos:

        <http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA>
        a                  dcatapit:Organization , vcard:Organization, vcard:Kind ;
        vcard:fn           "banche dati e open data" ;
        vcard:hasEmail     <mailto:info@dati.gov.it> ;
        vcard:hasTelephone [ a vcard:Voice ; vcard:value "06123456" ] ;
        vcard:hasURL       <http://spcdata.digitpa.gov.it/contattaci.html> .
