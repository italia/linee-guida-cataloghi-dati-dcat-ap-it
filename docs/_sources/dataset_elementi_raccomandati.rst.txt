Elementi raccomandati
=====================

Sottotema del dataset ``dct:subject``
-------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       0..N
Stato             Raccomandato
Descrizione       | La sottocategoria in cui può  essere  classificato  il  Dataset.
                  | La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a uno o più oggetti (codominio) di
                  | tipo skos:Concept (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/subject
================  ================================================================================


.. note::
    In corrispondenza del `tema scelto <temi.html>`__, si possono specificare più categorie per indicare parole chiave specifiche con cui il dataset può essere ulteriormente classificato.



Esempi di uso di ``dct:subject``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
           "dcterms:subject": [
            {
              "@id": "http://eurovoc.europa.eu/3193"
            },
            {
              "@id": "http://eurovoc.europa.eu/1810"
            }
          ],
          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
            <rdf:type rdf:resource="&dcat;Dataset"/>
            <dct:subject rdf:resource="http://eurovoc.europa.eu/3193"/>
            <dct:subject rdf:resource="http://eurovoc.europa.eu/1810"/>
            [altri elementi per specificare il dataset]
       </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                dcatapit:Dataset , dcat:Dataset ;
        dct:subject      <http://eurovoc.europa.eu/3193> , <http://eurovoc.europa.eu/1810> ;
        [altri elementi per specificare il dataset]




Punto di contatto del dataset ``dcat:contactPoint``
---------------------------------------------------

================  =================================================================================
elemento          valore
================  =================================================================================
Cardinalità       0..N
Stato             Raccomandato
Descrizione       | Il Punto di contatto del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a uno o più oggetti
                  | (codominio) di tipo `Punto di Contatto <punto-di-contatto.html>`__ (specificato
                  | mediante un URI - Uniform Resource Identifier)
Riferimento       http://www.w3.org/ns/dcat#contactPoint
================  =================================================================================



.. Note::
    Utilizzare questa proprietà per specificare le informazioni di contatto usate per inviare osservazioni, richieste di informazioni e commenti sul Dataset. **E' bene non confondere questo metadato con l'organizzazione titolare o editore o creatore del dataset. Il punto di contatto è usato tipicamente per specificare i riferimenti di un ufficio dell'organizzazione che può fornire informazioni sul dataset.** Si veda la sezione `Punto di Contatto. <punto-di-contatto.html>`__



Esempi di uso di ``dcat:contactPoint``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcat:contactPoint": {
            "@id": "http://dati.gov.it/resource/PuntoContatto/contactPointContrattiSPC"
          },

          altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dcat:contactPoint rdf:resource="http://dati.gov.it/resource/PuntoContatto/contactPointContrattiSPC"/>
        [altri elementi per specificare il dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                  dcatapit:Dataset , dcat:Dataset ;
        dcat:contactPoint  <http://dati.gov.it/resource/PuntoContatto/contactPointContrattiSPC> ;
        [altri elementi per specificare il dataset]


Editore del dataset ``dct:publisher``
-------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       0..1
Stato             Raccomandato
Descrizione       | L'editore del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a un oggetto (codominio) di
                  | tipo `Agent (Soggetto) <organizzazione.html>`__ (specificato mediante
                  | un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/publisher
================  ================================================================================



.. Note::
    Un'organizzazione (o pubblica amministrazione) responsabile di rendere disponibile (pubblicare) il dataset. **Si raccomanda di evitare l'inserimento di nomi di singole persone.** Si vedano gli `esempi riportati sull'uso della classe Agent. <organizzazione_esempi.html>`__



Esempi d'uso di ``dct:publisher``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
           "dcterms:publisher": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },

          altri elementi che descrivono il dataset

          Dove l'organizzazione editore è definita come:

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


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
     <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:publisher rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        [altri elementi del dataset]
     </dcatapit:Dataset>

     Dove l'organizzazione editore è descritta come:
     <!-- http://dati.gov.it/resource/Amministrazione/agid -->
     <dcatapit:Agent rdf:about="http://dati.gov.it/resource/Amministrazione/agid">
        <rdf:type rdf:resource="&foaf;Agent"/>
        <dct:identifier>agid</dct:identifier>
        <foaf:name xml:lang="it">Agenzia per l'Italia Digitale</foaf:name>
     </dcatapit:Agent>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a              dcatapit:Dataset , dcat:Dataset ;
        dct:publisher  <http://dati.gov.it/resource/Amministrazione/agid> ;
        [altri elementi del dataset] .

     Dove l'organizzazione editore è definita come:
     <http://dati.gov.it/resource/Amministrazione/agid>
        a               dcatapit:Agent , foaf:Agent ;
        dct:identifier  "agid" ;
        foaf:name       "Agenzia per l'Italia Digitale" .
