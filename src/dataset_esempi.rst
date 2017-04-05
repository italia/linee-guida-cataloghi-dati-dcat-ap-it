Esempi
======

Esempi per  ``dcatapit:Dataset``


``JSON-LD``

.. code-block:: json
   :linenos:

     {
          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcat:contactPoint": {
            "@id": "http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA"
          },
          "dcat:distribution": {
            "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti-N3"
          },
          "dcat:keyword": [
            "Contratto pubblico",
            "SPC",
            "Acquisizione"
          ],
          "dcat:theme": {
            "@id": "http://publications.europa.eu/resource/authority/data-theme/ECON"
          },
          "dcterms:accrualPeriodicity": {
            "@id": "http://publications.europa.eu/resource/authority/frequency/NEVER"
          },
          "dcterms:creator": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },
          "dcterms:description": {
            "@language": "it",
            "@value": "Il dataset LOD che contiene i contratti SPC del Lotto 1 (2007)"
          },
          "dcterms:identifier": "agid:D.301",
          "dcterms:modified": {
            "@type": "xsd:date",
            "@value": "2015-05-25"
          },
          "dcterms:publisher": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },
          "dcterms:rightsHolder": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },
          "dcterms:spatial": {
            "@id": "http://www.geonames.org/3169070"
          },
          "dcterms:subject": [
            {
              "@id": "http://eurovoc.europa.eu/3193"
            },
            {
              "@id": "http://eurovoc.europa.eu/1810"
            }
          ],
          "dcterms:temporal": {
            "@id": "http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC"
          },
          "dcterms:title": {
            "@language": "it",
            "@value": "Contratti del Sistema Pubblico di Connettività (SPC)"
          }
        },


``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->

      <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:modified rdf:datatype="&xsd;date">2015-05-25</dct:modified>
        <dct:identifier>agid:D.301</dct:identifier>
        <dcat:keyword>Acquisizione</dcat:keyword>
        <dcat:keyword>SPC</dcat:keyword>
        <dcat:keyword>Contratto pubblico</dcat:keyword>
        <dct:title xml:lang="it">Contratti del Sistema Pubblico di Connettività (SPC)</dct:title>
        <dct:description xml:lang="it">Il dataset contiene i contratti SPC del Lotto 1 (2007)</dct:description>
        <dct:publisher rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        <dct:creator rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        <dct:rightsHolder rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        <dcat:distribution rdf:resource="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3"/>
        <dcat:contactPoint rdf:resource="http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA"/>
        <dct:temporal rdf:resource="http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC"/>
        <dct:subject rdf:resource="http://eurovoc.europa.eu/3193"/>
        <dct:subject rdf:resource="http://eurovoc.europa.eu/1810"/>
        <dcat:theme rdf:resource="http://publications.europa.eu/resource/authority/data-theme/ECON"/>
        <dct:accrualPeriodicity rdf:resource="http://publications.europa.eu/resource/authority/frequency/NEVER"/>
        <dct:spatial rdf:resource="http://www.geonames.org/3169070"/>
      </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                       dcatapit:Dataset , dcat:Dataset ;
        dct:identifier          "agid:D.301" ;
        dct:title               "Contratti del Sistema Pubblico di Connettività (SPC)"@it ;
        dct:description         "Il dataset contiene i contratti SPC del Lotto 1 (2007)"@it ;
        dcat:theme              <http://publications.europa.eu/resource/authority/data-theme/ECON> ;
        dct:subject             <http://eurovoc.europa.eu/3193> , <http://eurovoc.europa.eu/1810>;
        dct:modified            "2015-05-25"^^xsd:date ;
        dcat:keyword            "Acquisizione" , "Contratto pubblico" , "SPC" ;
        dct:rightsHolder        <http://dati.gov.it/resource/Amministrazione/agid> ;
        dct:creator             <http://dati.gov.it/resource/Amministrazione/agid> ;
        dct:publisher           <http://dati.gov.it/resource/Amministrazione/agid> ;
        dcat:distribution       <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3> ;
        dct:accrualPeriodicity  <http://publications.europa.eu/resource/authority/frequency/NEVER> ;
        dcat:contactPoint       <http://dati.gov.it/resource/PuntoContatto/contactPointLODIPA> ;
        dct:spatial             <http://www.geonames.org/3169070> ;
        dct:temporal            <http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC> .
