Esempi
======

Esempi d'uso di ``adms:Identifier``


``JSON-LD``

.. code-block:: json
   :linenos:

       {
          "@id": "http://dati.gov.it/resource/AltroIdentificativo/altroidentificativoDataset1",
          "@type": "adms:Identifier",
          "skos:notation": {
            "@value": "doi:10.1109/5.771073"
          }
        }



``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/AltroIdentificativo/altroidentificativoDataset1 -->
      <adms:Identifier rdf:about="http://dati.gov.it/resource/AltroIdentificativo/altroidentificativoDataset1">
          <skos:notation>"doi:10.1109/5.771073"</skos:notation>
      </adms:Identifier>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <hhttp://dati.gov.it/resource/AltroIdentificativo/altroidentificativoDataset1>
        a               adms:Identifier ;
        skos:notation   "doi:10.1109/5.771073" ;
