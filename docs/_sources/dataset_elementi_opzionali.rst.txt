Elementi opzionali
==================


Autore del dataset ``dct:creator``
----------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Il creatore del Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html> a uno o più oggetti (codominio) di tipo
                  | `Agent (Soggetto) <organizzazione.html>`__ (specificato mediante un
                  | URI - Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/creator
================  ===================================================================================================


.. Note::
    Un'organizzazione (o pubblica amministrazione) che ha materialmente prodotto il dataset. **Si raccomanda di evitare l'inserimento di nomi di singole persone.** Si vedano gli `esempi riportati sull'uso della classe Agent (Soggetto). <organizzazione_esempi.html>`__



Esempi di uso di ``dct:creator``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
           "dcterms:creator": {
            "@id": "http://dati.gov.it/resource/Amministrazione/agid"
          },

          altri elementi che descrivono il dataset

          Dove l'amministrazione creatore è specificata come:
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
        <dct:creator rdf:resource="http://dati.gov.it/resource/Amministrazione/agid"/>
        [altri elementi del dataset]
     </dcatapit:Dataset>

     Dove l'amministrazione creatore è specificata come:
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
        a            dcatapit:Dataset , dcat:Dataset ;
        dct:creator  <http://dati.gov.it/resource/Amministrazione/agid> ;
        [altri elementi del dataset] .

     Dove l'amministrazione creatore è specificata come:
     <http://dati.gov.it/resource/Amministrazione/agid>
        a               dcatapit:Agent , foaf:Agent ;
        dct:identifier  "agid" ;
        foaf:name       "Agenzia per l'Italia Digitale"




Versione del dataset ``owl:versionInfo``
----------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       La versione del Dataset
Riferimento       http://www.w3.org/2002/07/owl#versionInfo
================  ===================================================================================================



.. note::
    Utilizzato per specificare il numero della versione o altre indicazioni della versione del dataset. **Per indicare il numero della versione, è fortemente raccomandato l’utilizzo di numeri separati dal “.”.** **Esempi** --> 0.7, 1.2.3, 1.10



Esempi di uso di ``owl:versionInfo``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
            "owl:versionInfo": "2.0"
         },

          altri elementi che descrivono il dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

     <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
     <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <owl:versionInfo>2.0</owl:versionInfo>
        [altri elementi del dataset]
     </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                dcatapit:Dataset , dcat:Dataset ;
        owl:versionInfo  "2.0" ;
        [altri elementi del dataset]




Data rilascio dataset ``dct:issued``
------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       La data di rilascio del Dataset
Riferimento       http://purl.org/dc/terms/issued
================  ===================================================================================================



.. note::
    E' la data in cui il dataset è reso disponibile.



Esempi di uso di ``dct:issued``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:

		"@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC\_agid",
    "@type": [
		    "dcat:Dataset", "http://dati.gov.it/onto/dcatapit#"Dataset"
    ],
		"dcterms:issued": {
       "@type": "xsd:date", "
       @value": "2012-01-15"
    }
    ltri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:issued rdf:datatype="&xsd;date">2012-01-15</dct:issued>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
	    a           dcatapit:Dataset , dcat:Dataset ;
	    dct:issued  "2012-01-15"^^xsd:date ;
	    [altri elementi del dataset]



Pagina di accesso del dataset ``dcat:landingPage``
--------------------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..1
Stato             Opzionale
Descrizione       | La pagina di accesso o landing page del Dataset. La proprietà lega l'oggetto
                  | (dominio) `Dataset <dataset.html>`__ a un oggetto (codominio) di tipo foaf:Document
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       https://www.w3.org/ns/dcat#landingPage
================  ===================================================================================================


.. note::
    Si raccomanda di utilizzare l’URL della pagina web che fornisce l’accesso al dataset o alla sua distribuzione o ad altre informazioni aggiuntive. La pagina di accesso è quella di origine del fornitore del dato. Non è valido l’URL di una pagina web riferibile a un sito fornito da una terza parte, come nel caso di un aggregatore.



Esempi d'uso di ``dcat:landingPage``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
            "dcat:landingPage": {
            "@id": "http://spcdata.digitpa.gov.it/dataLotto1.html"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
          <rdf:type rdf:resource="&dcat;Dataset"/>
          <dcat:landingPage rdf:resource="http://spcdata.digitpa.gov.it/dataLotto1.html />
          [altri elementi del dataset]
       </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                dcatapit:Dataset , dcat:Dataset ;
        dcat:landingPage <http://spcdata.digitpa.gov.it/dataLotto1.html> ;
        [altri elementi del dataset]




Lingua del dataset ``dct:language``
-----------------------------------


================  ===========================================================================================================
elemento          valore
================  ===========================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | La lingua del Dataset. La proprietà lega l'oggetto (dominio)
			            | `Dataset <dataset.html>`__ a uno o più oggetti (codominio) di tipo dct:LinguisticSystem
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/language
================  ===========================================================================================================


.. note::
    Indicaare una o più lingue utilizzate nel dataset. La scelta della lingua è regolata **dall'uso obbligatorio** del `vocabolario definito a livello Europeo sulle lingue. <http://publications.europa.eu/mdr/resource/authority/language/skos/languages-skos.rdf>`__ 



Esempi di uso di ``dct:language``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:language": {
            "@id": "http://publications.europa.eu/resource/authority/language/ITA"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:language rdf:resource="http://publications.europa.eu/resource/authority/language/ITA"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a              dcatapit:Dataset , dcat:Dataset ;
        dct:language   <http://publications.europa.eu/resource/authority/language/ITA> ;

        [altri elementi del dataset]




Parole chiave dataset ``dcat:keyword``
--------------------------------------


================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       La parole chiave associate al Dataset
Riferimento       https://www.w3.org/ns/dcat#keyword
================  ===================================================================================================


.. note::
    inserire una o più parole chiave che consentono di identificare l'oggetto principale del dataset. Se si è scelto di inserire un tema più specifico per il dataset (soggetto o sotto tema) assicurarsi che le parole chiave siano allineate ai temi e sotto temi usati, derivanti dai relativi vocabolari controllati. **Si ricorda che nella definizione delle parole chiave non sono ammessi alcuni caratteri come la virgola, l'apostrofo, la "/" e altri caratteri non alfanumerici. Pertanto NON sono ammesse parole chiave come "controllo della qualità dell'aria" oppure "cave dismesse, cave" oppure "legge 190/2012". In questi casi si suggerisce di sostituirle rispettivamente con "controllo qualità aria" ovvero togliendo testo superfluo, "cave dismesse" "cave" ovvero separando le diverse parole chiave, "legge 190-2012" ovvero inserendo un "-", ecc.**



Esempi di uso di ``dcat:keyword``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
            "dcat:keyword": [
            "Contratto pubblico",
            "SPC",
            "Acquisizione"
          ],

          altri elementi del dataset


``RDF/XML``

.. code-block:: turtle
   :linenos:


       <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
       <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
            <rdf:type rdf:resource="&dcat;Dataset"/>
            <dcat:keyword>Acquisizione</dcat:keyword>
            <dcat:keyword>SPC</dcat:keyword>
            <dcat:keyword>Contratto pubblico</dcat:keyword>
            [altri elementi del dataset]
        </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a              dcatapit:Dataset , dcat:Dataset ;
        dcat:keyword   "Acquisizione" , "Contratto pubblico" , "SPC" ;
        [altri elementi del dataset]



Dataset correlato ``dct:isVersionOf``
-------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Un Dataset correlato che è una versione, un’edizione o un adattamento del
                  | Dataset descritto. La proprietà lega l'oggetto (dominio) `Dataset <dataset.html>`__ a uno o più
                  | oggetti (codominio) di tipo `Dataset <dataset.html>`__ (specificato mediante un
                  | URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/isVersionOf
================  ===================================================================================================



.. note::
    Utilizzare l'URI del dataset correlato, ovvero il riferimento a una versione, un’edizione, un adattamento del dataset descritto. Per esempio, se si vuole inserire una nuova versione 2.0 di un dataset già presente nel catalogo (con versione 1.0) si richiede di indicare il riferimento al dataset già incluso nel catalogo. **Si sconsiglia fortemente comunque di creare nuovi dataset per piccoli cambiamenti. E’ invece consigliato definire nuovi dataset solo in presenza di cambiamenti significativi rispetto a precedenti versioni (e.g., nuovi elementi inclusi, adattamenti significativi di alcuni elementi, ecc).**



Esempi d'uso di ``dct:isVersionOf``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          ""dcterms:isVersionOf": {
            "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid01"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:isVersionOf rdf:resource="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid01"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <<http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a               dcatapit:Dataset , dcat:Dataset ;
        dct:isVersionOf <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid01> ;

        [altri elementi del dataset]


Estensione temporale del dataset ``dct:temporal``
-------------------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Un periodo temporale coperto dal Dataset. La proprietà lega l'oggetto
                  | (dominio) `Dataset <dataset.html>`__ a uno o più oggetti (codominio)
                  | di tipo `Periodo di Tempo <copertura-temporale.html>`__ (specificato mediante
                  | un URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/temporal
================  ===================================================================================================


.. note::
    Questo metadato è utilizzato per rappresentare, per esempio, casi quali “il dataset sul censimento della popolazione residente del 2011” oppure “il dataset sulla spesa pubblica dal 2000 al 2015". Per l'uso pratico di questa proprietà si vedano gli `esempi d'uso per la copertura temporale del Dataset. <copertura-temporale_esempi.html>`__



Esempi d'uso di ``dct:temporal``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:temporal": {
            "@id": "http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:temporal rdf:resource="http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <<http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a             dcatapit:Dataset , dcat:Dataset ;
        dct:temporal  <http://dati.gov.it/resource/PeriodoTemporale/periodTimeContrattiSPC> ;

        [altri elementi del dataset]




Copertura geografica del dataset ``dct:spatial``
------------------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Un'area geografica coperta dal Dataset. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a uno o più oggetti (codominio) di tipo
                  | `Localizzazione <copertura-geografica.html>`__ (specificato mediante un
                  | URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/spatial
================  ===================================================================================================


.. note::
    Per l'uso pratico di questa proprietà si vedano gli `esempi d'uso per la copertura geografica del Dataset <copertura-geografica_esempi.html>`__



Esempi d'uso di ``dct:spatial``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:


          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:spatial": {
            "@id": "http://www.geonames.org/3169070"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:spatial rdf:resource="http://www.geonames.org/3169070"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a           dcatapit:Dataset , dcat:Dataset ;
        dct:spatial <http://www.geonames.org/3169070> ;

        [altri elementi del dataset]



Conformità del dataset ``dct:conformsTo``
-----------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Una regola implementativa o altra specifica (e.g., una norma) a cui il
                  | Dataset è conforme. La proprietà lega l'oggetto (dominio)
                  | `Dataset <dataset.html>`__ a un o più oggetti (codominio) di tipo `Standard <standard.html>`__
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://purl.org/dc/terms/conformsTo
================  ===================================================================================================


.. note::
    Specificare uno o più standard riferibili al dataset. Si possono specificare sia standard tecnici (anche de-facto) come per esempio DCAT, ISO/IEC 25012, CSW, ecc., sia riferimenti normativi (e.g., Decreto legislativo n.82/2005 - Codice dell’Amministrazione Digitale). Per l'uso pratico di questa proprietà si vedano gli `esempi d'uso per lo Standard del Dataset <standard_esempi.html>`__



Esempi di uso di ``dct:conformsTo``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "dcterms:conformsTo": {
            "@id": "http://dati.gov.it/resource/Standard/standard-org"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dct:conformsTo rdf:resource="http://dati.gov.it/resource/Standard/standard-org"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <<http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a               dcatapit:Dataset , dcat:Dataset ;
        dct:conformsTo  <http://dati.gov.it/resource/Standard/standard-org> ;

        [altri elementi del dataset]


Altro identificativo del dataset ``adms:identifier``
----------------------------------------------------

================  ===================================================================================================
elemento          valore
================  ===================================================================================================
Cardinalità       0..N
Stato             Opzionale
Descrizione       | Un eventuale identificativo secondario del Dataset (e.g., DOI, ISBN, W3ID, ecc.).
                  | La proprietà lega l'oggetto (dominio) `Dataset <dataset.html>`__ a uno o più oggetti
                  | (codominio) di tipo `Altro Identificativo <identificativo-alternativo.html>`__
                  | (specificato mediante un URI- Uniform Resource Identifier)
Riferimento       http://www.w3.org/ns/adms#identifier
================  ===================================================================================================

.. note::
    Specificare uno o più identificativi secondari per il dataset. Per esempio, un identificativo secondario può essere un identificativo DOI (e.g., doi:10.10.1038/nphys1170) oppure un identificativo permanente per il Web W3ID (e.g., http://w3id.org/food) **oppure un identificativo stabile utilizzato in cataloghi locali**. Per l'uso pratico di questa proprietà si vedano gli `esempi d'uso per l'Identificativo Alternativo del Dataset <identificativo-alternativo_esempi.html>`__



Esempi di uso di ``adms:identifier``
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^



``JSON-LD``

.. code-block:: json
   :linenos:

          "@id": "http://dati.gov.it/resource/Dataset/ContrattiSPC_agid",
          "@type": [
            "dcat:Dataset",
            "http://dati.gov.it/onto/dcatapit#\"Dataset"
          ],
          "adms:identifier": {
            "@id": "http://dati.gov.it/resource/Identifier/ContrattiSPC_agid_altroID"
          },

          altri elementi del dataset


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/Dataset/ContrattiSPC_agid -->
    <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <adms:identifier rdf:resource="http://dati.gov.it/resource/Identifier/ContrattiSPC_agid_altroID"/>
        [altri elementi del dataset]
    </dcatapit:Dataset>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

     <<http://dati.gov.it/resource/Dataset/ContrattiSPC_agid>
        a                dcatapit:Dataset , dcat:Dataset ;
        adms:identifier  <http://dati.gov.it/resource/Identifier/ContrattiSPC_agid_altroID> ;

       [altri elementi del dataset]
