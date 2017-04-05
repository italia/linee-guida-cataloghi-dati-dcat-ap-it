Esempi
======

Esempi d'uso per ``dct:PeriodOfTime``


``JSON-LD``

.. code-block:: json
   :linenos:

       {
          "@id": "http://dati.gov.it/resource/PeriodoTemporale/periodTimeLinkedOpenIPA",
          "@type": "dcterms:PeriodOfTime",
          "http://dati.gov.it/onto/dcatapit#\"startDate": {
            "@type": "xsd:date",
            "@value": "2016-01-01"
          }
        }


``RDF/XML``

.. code-block:: xml
   :linenos:


    <!-- http://dati.gov.it/resource/PeriodoTemporale/periodTimeLinkedOpenIPA -->
    <dct:PeriodOfTime rdf:about="http://dati.gov.it/resource/PeriodoTemporale/periodTimeLinkedOpenIPA">
        <dcatapit:startDate rdf:datatype="&xsd;date">2016-01-01</dcatapit:startDate>
    </dct:PeriodOfTime>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC>
        a                   dct:PeriodOfTime ;
        dcatapit:startDate  "2007-01-01"^^xsd:date ;
        dcatapit:endDate    "2012-12-31"^^xsd:date .
