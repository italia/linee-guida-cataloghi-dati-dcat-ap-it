Overview profilo
===========================

La tabella che segue riporta l’elenco delle classi e delle proprietà definite nel profilo italiano e il relativo livello di obbligatorietà; in particolare, “M” indica che la classe è obbligatoria, “R” indica che è raccomandata e “O” indica che è opzionale.

Esempi completi dell'uso del profilo sono comunque disponibili anche in ``dati.gov.it`` in `RDF/XML e  RDF/Turtle. <http://www.dati.gov.it/sites/default/files/esempi_0.zip>`__

======================================================================== ================================================================================================================================== ===========================
Classe                                                                   Proprietà                                                                                                                          Obbligatorietà (M, R, O)
======================================================================== ================================================================================================================================== ===========================
`CATALOGO <catalogo.html>`__                                                                                                                                                                                M
Catalogo                                                                 `titolo <catalogo_elementi_obbligatori.html#titolo-dct-title>`__                                                                   M
Catalogo                                                                 `descrizione <ccatalogo_elementi_obbligatori.html#descrizione-dct-description>`__                                                  M
Catalogo                                                                 `editore <catalogo_elementi_obbligatori.html#editore-dct-publisher>`__                                                             M
Catalogo                                                                 `data ultima modifica <catalogo_elementi_obbligatori.html#data-ultima-modifica-dct-modified>`__                                    M
Catalogo                                                                 `dataset <catalogo_elementi_obbligatori.html#dataset-dcat-dataset>`__                                                              M
Catalogo                                                                 `home page <catalogo_elementi_raccomandati.html#homepage-foaf-homepage>`__                                                         R
Catalogo                                                                 `lingua <catalogo_elementi_raccomandati.html#lingua-dct-language>`__                                                               R
Catalogo                                                                 `data di rilascio <catalogo_elementi_raccomandati.html#data-di-rilascio-dct-issued>`__                                             R
Catalogo                                                                 `temi <catalogo_elementi_raccomandati.html#temi-dcat-themetaxonomy>`__                                                             R
`DATASET <dataset.html>`__                                                                                                                                                                                  M
Dataset                                                                  `identificativo <dataset_elementi_obbligatori.html#identificativo-del-dataset-dct-identifier>`__                                   M
Dataset                                                                  `titolo <dataset_elementi_obbligatori.html#titolo-del-dataset-dct-title>`__                                                        M
Dataset                                                                  `descrizione <dataset_elementi_obbligatori.html#descrizione-del-dataset-dct-description>`__                                        M
Dataset                                                                  `data ultima modifica <dataset_elementi_obbligatori.html#ultima-modifica-del-dataset-dct-modified>`__                              M
Dataset                                                                  `temi <dataset_elementi_obbligatori.html#temi-del-dataset-dcat-theme>`__                                                           M
Dataset                                                                  `titolare <dataset_elementi_obbligatori.html#titolare-del-dataset-dct-rightsholder>`__                                             M
Dataset                                                                  `frequenza di aggiornamento <dataset_elementi_obbligatori.html#frequenza-aggiornamento-dataset-dct-accrualperiodicity>`__          M
Dataset                                                                  `distribuzione <dataset_elementi_obbligatori.html#distribuzione-del-dataset-dcat-distribution>`__                                  M (nel caso di dati aperti)
Dataset                                                                  `sottotema <dataset_elementi_raccomandati.html#sottotema-del-dataset-dct-subject>`__                                               R
Dataset                                                                  `punto di contatto <dataset_elementi_raccomandati.html#punto-di-contatto-del-dataset-dcat-contactpoint>`__                         R
Dataset                                                                  `editore <dataset_elementi_raccomandati.html#editore-del-dataset-dct-publisher>`__                                                 R
Dataset                                                                  `autore <dataset_elementi_opzionali.html#autore-del-dataset-dct-creator>`__                                                        O
Dataset                                                                  `versione <dataset_elementi_opzionali.html#versione-del-dataset-owl-versioninfo>`__                                                O
Dataset                                                                  `data di rilascio <dataset_elementi_opzionali.html#data-rilascio-dataset-dct-issued>`__                                            O
Dataset                                                                  `pagina di accesso <dataset_elementi_opzionali.html#pagina-di-accesso-del-dataset-dcat-landingpage>`__                             O
Dataset                                                                  `lingua <dataset_elementi_opzionali.html#lingua-del-dataset-dct-language>`__                                                       O
Dataset                                                                  `parole chiave <dataset_elementi_opzionali.html#parole-chiave-dataset-dcat-keyword>`__                                             O
Dataset                                                                  `dataset correlato <dataset_elementi_opzionali.html#dataset-correlato-dct-isversionof>`__                                          O
Dataset                                                                  `estensione temporale <dataset_elementi_opzionali.html#estensione-temporale-del-dataset-dct-temporal>`__                           O
Dataset                                                                  `copertura geografica <dataset_elementi_opzionali.html#copertura-geografica-del-dataset-dct-spatial>`__                            O
Dataset                                                                  `conformità <dataset_elementi_opzionali.html#conformita-del-dataset-dct-conformsto>`__                                             O
Dataset                                                                  `altro identificativo <dataset_elementi_opzionali.html#altro-identificativo-del-dataset-adms-identifier>`__                        O
`DISTRIBUZIONE <distribuzione.html>`__                                                                                                                                                                      M
Distribuzione                                                            `formato <distribuzione_elementi_obbligatori.html#formato-distribuzione-dct-format>`__                                             M
Distribuzione                                                            `URL di accesso <distribuzione_elementi_obbligatori.html#url-di-accesso-dcat-accessurl>`__                                         M
Distribuzione                                                             `licenza <distribuzione_elementi_obbligatori.html#licenza-dct-license>`__                                                          M
Distribuzione                                                            `descrizione <distribuzione_elementi_raccomandati.html#descrizione-distribuzione-dct-description>`__                               R
Distribuzione                                                            `titolo <distribuzione_elementi_opzionali.html#titolo-distribuzione-dct-title>`__                                                  O
Distribuzione                                                            `URL di download <distribuzione_elementi_opzionali.html#url-di-download-dcat-downloadurl>`__                                       O
Distribuzione                                                            `data ultima modifica <distribuzione_elementi_opzionali.html#ultima-modifica-distribuzione-dct-modified>`__                        O
Distribuzione                                                            `dimensione in byte <distribuzione_elementi_opzionali.html#dimensione-in-byte-dcat-bytesize>`__                                    O
`SOGGETTO <organizzazione.html#>`__                                                                                                                                                                         M
Soggetto                                                                 `identificativo <organizzazione_elementi_obbligatori.html#identificativo-del-soggetto-dct-identifier>`__                           M
Soggetto                                                                 `nome <organizzazione_elementi_obbligatori.html#nome-del-soggetto-foaf-name>`__                                                    M
`IDENTIFICATIVO ALTERNATIVO <identificativo-alternativo.html>`__                                                                                                                                            O
identificativo alternativo                                               `notazione <identificativo-alternativo_elementi_raccomandati.html#notazione-skos-notation>`__                                      R
`LICENZA <licenza.html>`__                                                                                                                                                                                  M
Licenza                                                                  `tipo <licenza_elementi_raccomandati.html#tipo-licenza-dct-type>`__                                                                R
Licenza                                                                  `nome <licenza_elementi_opzionali.html#nome-licenza-foaf-name>`__                                                                  O
Licenza                                                                  `versione <licenza_elementi_opzionali.html#versione-licenza-owl-versioninfo>`__                                                    O
`PERIODO DI TEMPO <copertura-temporale.html>`__                                                                                                                                                             O
Periodo di tempo                                                         `data di inizio <copertura-temporale_elementi_obbligatori.html#data-inizio-dcatapit-startdate>`__                                  M
Periodo di tempo                                                         `data di fine <copertura-temporale_elementi_opzionali.html#data-inizio-dcatapit-enddate>`__                                        O
`STANDARD <standard.html>`__                                                                                                                                                                                O
Standard                                                                 `identificativo <standard_elementi_obbligatori.html#identificativo-dello-standar-dct-identifier>`__                                M
Standard                                                                 `titolo <standard_elementi_opzionali.html#titolo-dello-standard-dct-title>`__                                                      O
Standard                                                                 `descrizione <standard_elementi_opzionali.html#descrizione-dello-standard-dct-description>`__                                      O
Standard                                                                 `documentazione di riferimento <standard_elementi_opzionali.html#documentazione-di-riferimento-dcatapit-referencedocumentation>`__ O
`PUNTO DI CONTATTO (ORGANIZZAZIONE) <punto-di-contatto.html>`__                                                                                                                                             R
Punto di contatto (organizzazione)                                       `nome <punto-di-contatto_elementi_obbligatori.html#nome-punto-di-contatto-vcard-fn>`__                                             M
Punto di contatto (organizzazione)                                       `email <punto-di-contatto_elementi_obbligatori.html#email-punto-di-contatto-vcard-hasemail>`__                                     M
Punto di contatto (organizzazione)                                       `telefono <punto-di-contatto_elementi_opzionali.html#telefono-punto-di-contatto-vcard-hastelephone>`__                             O
Punto di contatto (organizzazione)                                       `sito <punto-di-contatto_elementi_opzionali.html#sito-punto-di-contatto-vcard-hasurl>`__                                           O
`LOCALIZZAZIONE <copertura-geografica.html>`__                                                                                                                                                              O
Localizzazione                                                           `nome geografico <copertura-geografica_elementi_opzionali.html>`__                                                                 O
Localizzazione                                                           `geometria <copertura-geografica_elementi_opzionali.html#geometria-loc-geometry>`__                                                O
`GEOMETRIA <copertura-geografica_elementi_obbligatori_geometria.html>`__                                                                                                                                    O
Geometria                                                                `crs <copertura-geografica_elementi_obbligatori_geometria.html#crs>`__                                                             M
Geometria                                                                `coordinate <copertura-geografica_elementi_obbligatori_geometria.html#coordinate>`__                                               M
Geometria                                                                `tipo di geometria <copertura-geografica_elementi_obbligatori_geometria.html#tipo-di-geometria>`__                                 M
======================================================================== ================================================================================================================================== ===========================
