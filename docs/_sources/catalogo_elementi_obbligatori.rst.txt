Elementi obbligatori
====================


Titolo ``dct:title``
--------------------

================  ============================================================================================
elemento          valore
================  ============================================================================================
**Cardinalità**   1..N (può esistere più di un'istanza in diverse lingue, della stessa proprietà)
**Stato**         Obbligatorio
**Descrizione**   Il titolo del Catalogo.
**RIferimento**   http://purl.org/dc/terms/title
================  ============================================================================================

.. note::

    Si raccomanda di inserire un testo **semplice e corto**. Si raccomanda di **non utilizzare acronimi o abbreviazioni incomprensibili**. Se si vogliono
    utilizzare comunque gli acronimi, riportare anche il nome esteso. Nel caso il catalogo sia parte di un progetto più ampio, si consiglia di indicare, tra parentesi,
    il nome del progetto alla fine del titolo stesso.
    **Esempio** --> "Catalogo dei dati aperti dell'AgID (Agenzia per l'Italia Digitale)" oppure "Catalogo delle banche dati della Regione Lazio".


Esempi d'uso di ``dct:title``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "dcterms:title": {
            "@language": "it",
            "@value": "Catalogo SPCData"
          },
          "dcterms:title": {
            "@language": "en",
            "@value": "SPCData Catalog"
          },

          altri elementi per specificere il catalogo



``RDF/XML``


.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->

    <rdf:Description rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#Catalog"/>
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dct:title xml:lang="it">Catalogo SPCData</dct:title>
        <dct:title xml:lang="en">SPCData Catalog</dct:title>
        [altri elementi per specificare il catalogo]
    </rdf:Description>


``RDF/Turtle``


.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a          dcatapit:Catalog , dcat:Catalog ;
        dct:title  "Catalogo Dati.gov.it"@it , "SPCData Catalog"@en ;

        [altri elementi per specificare il catalogo] .



Descrizione ``dct:description``
-------------------------------

================  ================================================================================
elemento          valore
================  ================================================================================
**Cardinalità**   1..N (può esistere più di un'istanza, in diverse lingue, della stessa proprietà)
**Stato**         Obbligatorio
**Descrizione**   La descrizione del Catalogo
**Riferimento**   http://purl.org/dc/terms/description
================  ================================================================================

 .. note::

	Si raccomanda di fornire una breve descrizione delle caratteristiche principali del catalogo. **Evitare di utilizzare un linguaggio ricco di riferimenti normativi. Utilizzare invece un linguaggio semplice che possa aiutare qualsiasi utente a identificare il catalogo**.Si ricorda che nessun tag HTML è consentito. **Esempio**--> "Il catalogo contiene i dati aperti dell'Agenzia per l'Italia Digitale, in particolare, i dati aperti dell'Indice della Pubblica Amministrazione (IPA) e dei contratti del Sistema Pubblico di Connettività (SPC) relativi alle gare del 2007".


Esempi d'uso di ``dct:description``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``


.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "dcterms:description": {
            "@language": "it",
            "@value": "Il catalogo dei dati aperti della pubblica amministrazione italiana"
          },

         altri elementi per specificare il catalogo


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->

    <rdf:Description rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
      <rdf:type rdf:resource="http://dati.gov.it/onto/dcatapit#Catalog"/>
      <rdf:type rdf:resource="&dcat;Catalog"/>
      <dct:description xml:lang="it">Il catalogo dei dati aperti della pubblica amministrazione italiana</dct:description>
      [altri elementi per specificare il catalogo]
    </rdf:Description>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    	<http://dati.gov.it/resource/Catalogp/datigov_agid>
        a                dcatapit:Catalog , dcat:Catalog ;
        dct:description  "Il catalogo dei dati aperti della pubblica amministrazione italiana"@it ;
        [altri elementi per specificare il catalogo] .




Editore ``dct:publisher``
-------------------------

============== ==============================================================================================
elemento       valore
============== ==============================================================================================
Cardinalità    1
Stato          Obbligatorio
Descrizione    | L'editore del Catalogo. La proprietà lega l'oggetto (dominio)
               | `Catalog (Catalogo) <catalogo.html>`__ a un oggetto (codominio) di tipo `Agent <organizzazione.html>`__
               | (specificato mediante un URI - Uniform Resource Identifier)
Riferimento    http://purl.org/dc/terms/publishe
============== ==============================================================================================


 .. note::

	Un'organizzazione (o pubblica amministrazione) responsabile di rendere disponibile (pubblicare) il catalogo. **Si raccomanda di evitare l'inserimento di nomi di singole persone.** Si vedano gli `esempi riportati sull'uso della classe Agente <organizzazione_esempi.html>`__



Esempi d'uso di ``dct:publisher``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
           "dcterms:publisher": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },

          altri elementi che descrivono il catalogo

          Dove l'amministrazione è definita come:
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

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->
     <dcatapit:Catalog rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dct:publisher rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        [altri elementi del catalogo]
     </dcatapit:Catalog>

     Dove l'amministrazione è definita come:
     <!-- http://dati.gov.it/resource/Amministrazione/agid -->
     <dcatapit:Agent rdf:about="http://dati.gov.it/resource/Amministrazione/agid">
        <rdf:type rdf:resource="&foaf;Agent"/>
        <dct:identifier>agid</dct:identifier>
        <foaf:name xml:lang="it">Agenzia per l'Italia Digitale</foaf:name>
     </dcatapit:Agent>


``RDF/Turtle``

.. code-block:: Turtle
   :linenos:

     <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a               dcatapit:Catalog , dcat:Catalog ;
        dct:publisher   <http://dati.gov.it/resource/Amministrazione/agid> ;
        [altri elementi del catalogo] .

     Dove l'amministrazione è definita come:
     <http://dati.gov.it/resource/Amministrazione/agid>
        a               dcatapit:Agent , foaf:Agent ;
        dct:identifier  "agid" ;
        foaf:name       "Agenzia per l'Italia Digitale" .




Data ultima modifica ``dct:modified``
-------------------------------------

============== =================================================================
elemento       valore
============== =================================================================
Cardinalità    1
Stato          Obbligatorio
Descrizione    La data di ultima modifica del Catalogo
Riferimento    http://purl.org/dc/terms/modified
============== =================================================================


 .. note::

	La data di ultima modifica del catalogo. E' la data in cui si verificano operazioni di modifica del catalogo (es. l’inserimento di un nuovo dataset nel catalogo, la modifica dei metadati del catalogo o di uno dei dataset in esso inclusi).


Esempi d'uso di ``dct:modified``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
            "dcterms:modified": {
            "@type": "xsd:date",
            "@value": "2016-03-20"
          },

          altri elementi del catalogo


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->
     <dcatapit:Catalog rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dct:modified rdf:datatype="&xsd;date">2016-03-20</dct:modified>
        [altri elementi del catalogo]
     </dcatapit:Catalog>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a             dcatapit:Catalog , dcat:Catalog ;
        dct:modified  "2016-03-20"^^xsd:date ;
        [altri elementi del catalogo] .



Dataset ``dcat:dataset``
------------------------

============== =======================================================================================
elemento       valore
============== =======================================================================================
Cardinalità    1
Stato          Obbligatorio
Descrizione    | E' una proprietà che lega un oggetto (dominio) `Catalog (Catalogo) <catalogo.html>`__
               | all'oggetto (codominio) `Dataset <dataset.html>`__ ed è utilizzata per elencare
			         | la lista di dataset presenti nel catalogo
Riferimento    https://www.w3.org/ns/dcat#dataset
============== =======================================================================================

 .. note::

	Indicare tante proprietà dcat:dataset quanti sono i dataset presenti nel catalogo


Esempi d'uso di ``dcat:dataset``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid",
          "@type": [
            "dcat:Catalog",
            "http://dati.gov.it/onto/dcatapit#\"Catalog"
          ],
          "dcat:dataset": [
            {
              "@id": "http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid"
            },
            {
              "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid"
            }
          ],

          altri elementi del catalogo


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid -->
     <dcatapit:Catalog rdf:about="http://dati.gov.it/resource/Catalogo/SPCDataCatalog_agid">
        <rdf:type rdf:resource="&dcat;Catalog"/>
        <dcat:dataset rdf:resource="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid"/>
        <dcat:dataset rdf:resource="http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid"/>
        [altri elementi del catalogo]
     </dcatapit:Catalog>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Catalogp/datigov_agid>
        a               dcatapit:Catalog , dcat:Catalog ;
        dcat:dataset    <http://dati.gov.it/resource/Dataset/LinkedOpenIPA20_agid> ;
        dcat:dataset    <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid> ;
        [altri elementi del catalogo] .
