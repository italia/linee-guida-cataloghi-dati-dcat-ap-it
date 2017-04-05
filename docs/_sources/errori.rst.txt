Errori comuni nell'uso di DCAT-AP_IT
====================================

Gestione degli URI
------------------

L'errore più diffuso riguarda la gestione degli URI. Si ricorda
che oggetti di tipo diverso devono avere URI differenti. Per esempio,
**NON** è corretto utilizzare lo stesso URI per definire il soggetto o
organizzazione che ha un certo ruolo (titolare, editore, creatore) su un
catalogo o dataset, e per definire il punto di contatto del dataset. I
due concetti sono diversi e devono avere URI diversi. Ci si riferisca
agli esempi di uso di Soggetto o Organizzazione e di Punto di Contatto
per maggiori dettagli.

Differenza tra Literal (valore) e URI
-------------------------------------

Molto spesso, soprattutto in
presenza di dati serializzati in RDF/XML si tende a confondere il
concetto di URI http://.... con una stringa che all'interno contiene un
URI "http://....". In quest'ultimo caso non si sta definendo un URI ma
un valore (detto Literal nel contesto RDF). Per esempio il seguente codice **è** corretto:

.. code:: xml

     <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
        <rdf:type rdf:resource="&dcat;Dataset"/>
        <dcat:theme rdf:resource="http://publications.europa.eu/resource/authority/data-theme/ECON"/>
     ...
     </dcatapit:Dataset>

.. error::
  Il seguente codice definirebbe il tema come una stringa che include un
  URI e **NON** è corretto rispetto alle specifiche riguardanti il tema
  del Dataset:

    .. code:: xml

        <dcatapit:Dataset rdf:about="http://dati.gov.it/resource/Dataset/ContrattiSPC_agid">
            <rdf:type rdf:resource="&dcat;Dataset"/>
            <dcat:theme>"http://publications.europa.eu/resource/authority/data-theme/ECON"</dcat:theme>
            ...
        </dcatapit:Dataset>
