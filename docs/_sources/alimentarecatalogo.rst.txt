Come alimentare un catalogo dati
================================

Nell'ambito delle linee guida AgID per la valorizzazione del patrimonio informativo pubblico, sono state individuate due modalità di alimentazione di un catalogo dati: *editor online* e *harvesting automatico*. Le modalità sono descritte nel seguito.

Editor
------
E' un'applicazione Web integrata nel catalogo per l'acquisizione e l'aggiornamento guidato dei metadati. L'editor, acceduto tipicamente previa autenticazione, alimenta automaticamente il catalogo in modo da garantire la conformità al profilo di metadatazione nazionale.

.. note::
  L'uso di tale modalità è consigliata in presenza di pochi dataset che hanno anche una frequenza di aggiornamento ampia (e.g., semestrale, annuale).
  Nell'ambito del catalogo nazionale dei dati aperti ``dati.gov.it`` questa funzionalità non è ancora attiva.

Alcune Pubbliche Amministrazioni stanno collaborando alla stesura di un `vademecum <https://docs.google.com/document/d/12Jg1xyA6yLBWnjZNsnF7mesHyOyIWO5CumwAN9bw_G4/edit>`__ per l'inserimento, via editor online integrato in piattaforme standard come `CKAN <https://ckan.org/>`__, dei metadati conformi al profilo nazionale di metadatazione DCAT-AP_IT.

Harvesting
----------
E' una funzionalità offerta dal catalogo per l'acquisizione e l'aggiornamento periodico dei metadati.
Nell'ambito del catalogo nazionale dei dati aperti ``dati.gov.it``, l'uso di tale funzionalità richiede che l'amministrazione comunichi, solo la prima volta, l'URL del catalogo e indichi la modalità di harvesting (e.g., RDF DCAT-AP\_IT, CKAN, CSW).
Sarà lo stesso catalogo nazionale che si occuperà successivamente di raccogliere periodicamente i metadati che descrivono i dati.

.. note::
  L'uso della modalità harvesting è consigliato in presenza di un numero elevato di dataset, soggetti anche a frequenti aggiornamenti.
