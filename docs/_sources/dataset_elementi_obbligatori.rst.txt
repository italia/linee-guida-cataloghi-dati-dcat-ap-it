Elementi obbligatori
====================

Identificativo del dataset ``dct:identifier``
---------------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       L'identificativo univoco del Dataset assegnato dal catalogo nazionale
Riferimento       http://purl.org/dc/terms/identifier
================  ================================================================================

.. note::
    L'identificativo univoco del dataset è assegnato dal catalogo nazionale ed è costituito da codiceIPA:D.numeroProgressivo. **Esempio**--> agid:D.1


Esempi d'uso di ``dct:identifier``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

      "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
      "@type": [
        "dcat:Dataset",
        "http://dati.gov.it/onto/dcatapit#\"Dataset"
      ],
      "dcterms:identifier": "agid:D.301",

      altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->

      <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:identifier>agid:D.1</dct:identifier>
        [altri elementi per specificare il dataset]
      </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
            a                dcatapit:Dataset , dcat:Dataset ;
            dct:identifier   "agid:D.1" ;

            [altri elementi per specificare il dataset]



Titolo del dataset ``dct:title``
--------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Obbligatorio
Descrizione       Il titolo del Dataset
Riferimento       http://purl.org/dc/terms/title
================  ================================================================================


  .. note::

    Si raccomanda di inserire un testo **semplice e corto**. Si raccomanda di non utilizzare acronimi o abbreviazioni incomprensibili. Se si vogliono utilizzare comunque gli acronimi, riportare anche il nome esteso. Nel caso il dataset sia legato a un progetto più ampio, si consiglia di indicare, tra parentesi, il nome del progetto alla fine del titolo stesso. Si può evitare di inserire nel titolo del Dataset la distribuzione dello stesso (e.g., si può evitare di scrivere un titolo come "Luoghi ed eventi della cultura in LOD"). **Esempi di titoli di dataset** --> "Contratti del Sistema Pubblico di Connettività (SPC)" oppure "Luoghi ed eventi della cultura".



Esempi di uso di ``dct:title``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

      "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
      "@type": [
        "dcat:Dataset",
        "http://dati.gov.it/onto/dcatapit#\"Dataset"
      ],
      "dcterms:title": {
        "@language": "it",
        "@value": "Contratti del Sistema Pubblico di Connettività (SPC)"
      },

      altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

      <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->

      <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:title xml:lang="it">Contratti del Sistema Pubblico di Connettività (SPC)</dct:title>
        [altri elementi per specificare il dataset]
      </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
          a            dcatapit:Dataset , dcat:Dataset ;
          dct:title    "Contratti del Sistema Pubblico di Connettività (SPC)"@it ;

          [altri elementi per specificare il dataset]



Descrizione del dataset ``dct:description``
-------------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
Stato             Obbligatorio
Descrizione       La descrizione del Dataset che indica cosa contiene il dataset.
Riferimento       http://purl.org/dc/terms/description
================  ================================================================================



 .. note::

   Si raccomanda di fornire una **breve descrizione dei contenuti principali del dataset. Evitare di utilizzare un linguaggio ricco di riferimenti normativi. Utilizzare invece un linguaggio semplice che possa aiutare qualsiasi utente a identificare il contenuto del dataset**. Ove possibile, si possono fornire indicazioni sulla struttura dei dati che compongono il dataset. Si ricorda che nessun tag HTML è consentito. **Esempi**--> "Il dataset contiene i dati sui contratti del Sistema Pubblico di Connettività (SPC) relativi al Lotto 1 dell'anno 2007." oppure "Il dataset contiene i dati relativi ai luoghi della cultura (e.g., musei, biblioteche, siti archeologici, ecc.) e i relativi eventi culturali che si tengono nei luoghi. Informazioni sugli orari di apertura per i luoghi e i relativi eventi sono incluse nel dataset".



Esempi di uso di ``dct:description``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:description": {
            "@language": "it",
            "@value": "Il dataset contiene i dati sui contratti del Sistema Pubblico di
                       Connettività (SPC) relativi al Lotto 1 dell'anno 2007"
          },

          altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
          <rdf:type rdf:resource="&dcat;Dataset"/>
          <dct:description xml:lang="it">Il dataset contiene i dati sui contratti del Sistema Pubblico di Connettività (SPC) relativi al Lotto 1 dell'anno 2007.</dct:description>
          [altri elementi per specificare il dataset]
       </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a               dcatapit:Dataset , dcat:Dataset ;
        dct:description "Il dataset contiene i dati sui contratti del Sistema Pubblico di
                         Connettività (SPC) relativi al Lotto 1 dell'anno 2007."

       [altri elementi per specificare il dataset]





Ultima modifica del dataset ``dct:modified``
--------------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       La data di ultima modifica del Dataset
Riferimento       http://purl.org/dc/terms/modified
================  ================================================================================



 .. note::

   Si raccomanda di usare il formato ISO 8601, i.e., yyyy-mm-dd



Esempi di uso di ``dct:modified``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:modified": {
            "@type": "xsd:date",
            "@value": "2015-05-25"
          },

          altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
            <rdf:type rdf:resource="&dcat;Dataset"/>
            <dct:modified rdf:datatype="&xsd;date">2015-05-25</dct:modified>
            [altri elementi per specificare il dataset]
       </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a               dcatapit:Dataset , dcat:Dataset ;
        dct:modified    "2015-05-25"^^xsd:date ;

        [altri elementi per specificare il dataset]



Temi del dataset ``dcat:theme``
-------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1..N
Stato             Obbligatorio
Descrizione       | I temi attraverso cui classificare il Dataset. La proprietà lega l'oggetto
                  | (dominio) `Dataset <dataset.html>`__ a uno o più
                  | oggetti (codominio) di tipo skos:Concept
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://www.w3.org/ns/dcat#theme
================  ================================================================================



.. note::

   Il metadato assume come valore un URI (NON una stringa con l'URL del tema) che **deve essere necessariamente** uno tra quelli definiti nel `vocabolario Europeo sui Temi per i dati <http://publications.europa.eu/mdr/resource/authority/data-theme/skos/data-theme-skos.rdf>`__. **Esempio** --> se il tema è Agricoltura, Pesca e Politiche Forestali e Alimentari il valore di questa proprietà è necessariamente http://publications.europa.eu/resource/authority/data-theme/AGRI. Si veda a tal proposito la sezione `"Temi dei dati" <temi.html>`__


Esempi d'uso di ``dcat:theme``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          {
           "@id": "http://publications.europa.eu/resource/authority/data-theme/ECON",
           "@type": "skos:Concept",
           "skos:prefLabel": {
             "@language": "it",
             "@value": "Economia e Finanze"
          }
        },

         altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
            <rdf:type rdf:resource="&dcat;Dataset"/>
            <dcat:theme rdf:resource="http://publications.europa.eu/resource/authority/data-theme/ECON"/>
            [altri elementi per specificare il dataset]
       </dcatapit:Dataset>

       Opzionalmente si può anche specificare
       <!-- http://publications.europa.eu/resource/authority/data-theme/ECON -->

       <skos:Concept rdf:about="http://publications.europa.eu/resource/authority/data-theme/ECON">
           <skos:prefLabel xml:lang="it">Economia e Finanze</skos:prefLabel>
       </skos:Concept>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a            dcatapit:Dataset , dcat:Dataset ;
        dcat:theme   <http://publications.europa.eu/resource/authority/data-theme/ECON> ;

        [altri elementi per specificare il dataset] .

      Opzionalmente si può anche specificare

      <http://publications.europa.eu/resource/authority/data-theme/ECON>
        a               skos:Concept ;
        skos:prefLabel  "Economia e Finanze"@it



Titolare del dataset ``dct:rightsHolder``
-----------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | Il titolare del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a un oggetto (codominio)
                  | di tipo `Agent (Soggetto) <organizzazione.html>`__
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/rightsHolder
================  ================================================================================


.. note::
    Il metadato assume come valore un URI (NON una stringa). Esso rappresenta un’organizzazione (o pubblica amministrazione) responsabile della gestione complessiva del dataset in virtù dei propri compiti istituzionali. **Si raccomanda di evitare l'inserimento di nomi di singole persone.** Si vedano gli `esempi riportati sull'uso della classe Agent (Soggetto) <organizzazione_esempi.html>`__


Esempi di uso di ``dct:rightsHolder``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
           "dcterms:rightsHolder": {
            "@id": "http://dati.gov.it/resource/Amministraione/agid"
          },
          altri elementi per specificare il dataset

          Dove l'Organizzazione http://dati.gov.it/resource/Amministraione/agid è definita come:

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

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
          <rdf:type rdf:resource="&dcat;Dataset"/>
          <dct:rightsHolder rdf:resource="http://dati.gov.it/resource/Amministraione/agid"/>
          [altri elementi per specificare il dataset]
       </dcatapit:Dataset>

       Dove l'organizzazione
       <!-- http://dati.gov.it/resource/Amministrazione/agid --> è definita come:

       <dcatapit:Agent rdf:about="http://dati.gov.it/resource/Amministrazione/agid">
          <rdf:type rdf:resource="&foaf;Agent"/>
          <dct:identifier>agid</dct:identifier>
          <foaf:name xml:lang="it">Agenzia per l'Italia Digitale</foaf:name>
       </dcatapit:Agent>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                 dcatapit:Dataset , dcat:Dataset ;
        dct:rightsHolder  <http://dati.gov.it/resource/Amministraione/agid> ;

        [altri elementi per specificare il dataset] .

     Dove l'organizzazione <http://dati.gov.it/resource/Amministraione/agid> è definita come

     <http://dati.gov.it/resource/Amministrazione/agid>
        a                 dcatapit:Agent , foaf:Agent ;
        dct:identifier    "agid" ;
        foaf:name         "Agenzia per l'Italia Digitale"





Frequenza aggiornamento dataset ``dct:accrualPeriodicity``
----------------------------------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
Cardinalità       1
Stato             Obbligatorio
Descrizione       | La frequenza di aggiornamento del Dataset. La proprietà lega l'oggetto
                  | (dominio) `Dataset <dataset.html>`__ a un oggetto
                  | (codominio) di tipo dct:Frequency
                  | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/accrualPeriodicity
================  ================================================================================

.. note::
   La frequenza con cui il dataset viene aggiornato **assume necessariamente** uno dei valori definiti nel `vocabolario Europeo sulle frequenze. <http://publications.europa.eu/mdr/resource/authority/frequency/skos/frequencies-skos.rdf>`__ **Esempio** --> se il dataset si aggiorna ogni trimestre il valore da indicare è http://publications.europa.eu/resource/authority/frequency/QUARTERLY. Nel caso la frequenza di aggiornamento non sia disponibile è possibile indicare una frequenza sconosciuta utilizzando il seguente URI: http://publications.europa.eu/resource/authority/frequency/UNKNOWN



Esempi d'uso di ``dct:accrualPeriodicity``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
            "dcterms:accrualPeriodicity": {
            "@id": "http://publications.europa.eu/resource/authority/frequency/ANNUAL_2"
          },

          altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
     <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:accrualPeriodicity rdf:resource="http://publications.europa.eu/resource/authority/frequency/ANNUAL_2"/>
        [altri elementi per specificare il dataset]
     </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                       dcatapit:Dataset , dcat:Dataset ;
        dct:accrualPeriodicity  <http://publications.europa.eu/resource/authority/frequency/ANNUAL_2> ;

        [altri elementi per specificare il dataset]



Distribuzione del dataset ``dcat:distribution``
-----------------------------------------------


================  =======================================================================================
elemento          valore
================  =======================================================================================
Cardinalità       1..N nel caso di dati aperti, 0..N negli altri casi
Stato             Obbligatorio nel caso di dati aperti, Opzionale negli altri casi
Descrizione       | La distribuzione del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a un oggetto (codominio)
                  | di tipo `Distribuzione <distribuzione.html>`__ (specificato mediante un URI - Uniform
                  | Resource Identifier)
Riferimento       http://www.w3.org/ns/dcat#distribution
================  =======================================================================================



.. note::
    Una distribuzione è una forma attraverso cui il dataset è disponibile. Ogni dataset può essere disponibile in diverse forme, come per esempio diversi formati o differenti endpoint (e.g., SPARQL endpoint). Nel caso di serie temporali o spaziali o viste di un dataset, queste sono descritte mediante le distribuzioni. Per esempio, nel caso di un dataset suddiviso per regioni, le suddivisioni rappresentano distribuzioni di un dataset più ampio che include tutti i dati del territorio nazionale. Si veda `Come definire una distribuzione <distribuzione.html>`__ per maggiori dettagli.



Esempi d'uso di ``dcat:distribution``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
           dcat:distribution": {
            "@id": "http://dati.gov.it/resource/Distribuzione/SPCContratti-N3"
          },

          altri elementi per specificare il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
          <rdf:type rdf:resource="&dcat;Dataset"/>
          <dcat:distribution rdf:resource="http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3"/>
          [altri elementi per specificare il dataset]
       </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

       <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                   dcatapit:Dataset , dcat:Dataset ;
        dcat:distribution   <http://dati.gov.it/resource/Distribuzione/SPCContratti_agid-N3> ;

        [altri elementi per specificare il dataset]
