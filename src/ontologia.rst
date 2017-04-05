Ontologia OWL di DCAT-AP_IT
===========================

E' stata definita `un'ontologia OWL <http://dati.gov.it/onto/dcatapit>`__ serializzata in RDF/XML e disponibile in ``dati.gov.it`` nella sezione ontologie (onto).
L’IRI dell’ontologia è http://dati.gov.it/onto/dcatapit

La scelta di creare un’ontologia OWL è dettata da diverse motivazioni.
In primo luogo è importante ribadire che **il profilo applicativo italiano** non è uno standard di per sé, ma **è un profilo di interoperabilità** derivato dal profilo europeo DCAT-AP. DCAT-AP, secondo quanto riportato dalle specifiche, a sua volta “*intende essere uno strumento da utilizzare in un ambiente di tipo Linked Data*”.
Evidenziare i benefici del paradigma dei Linked Data, soprattutto in relazione al raggiungimento di obiettivi di interoperabilità semantica, non rientra tra gli obiettivi di questa guida; a tal proposito i lettori interessati possono far riferimento alle `linee guida della Commissione di Coordinamento SPC pubblicate da AgID nel 2012 e intitolate “Interoperabilità semantica attraverso i Linked Open Data” <http://www.agid.gov.it/sites/default/files/documentazione_trasparenza/cdc-spc-gdl6-interoperabilitasemopendata_v2.0_0.pdf>`__. Tuttavia, **è importante sottolineare l’importanza della definizione di un’ontologia OWL**.

Le ontologie si stanno sempre più sviluppando come **strumento formale di rappresentazione**, sulla base di specifici requisiti, **di un dominio di conoscenza**. In particolare, al fine di massimizzare la condivisione della conoscenza e garantire interoperabilità semantica, **l’ontologia consente di descrivere la semantica dei dati** con una terminologia concordata che può essere poi successivamente riusata anche in altri contesti con simili obiettivi. Tipicamente **l’ontologia** non è un obiettivo di per sé ma **costituisce una base solida per poter sviluppare**, al di sopra di essa, **applicazioni e servizi avanzati semantici**, sempre più diffusi con lo sviluppo dei **Linked Data** e in ambito World Wide Web.

Secondo diversi ricercatori del settore, nel creare vocabolari e/o profili di interoperabilità (come nel caso di DCAT-AP e DCAT-AP_IT), è importante seguire determinati principi che consentono una pubblicazione virtuosa degli stessi. I principi sono derivati da quelli del paradigma Linked Data. Pertanto, nella creazione di vocabolari, profili di interoperabiiltà e ontologie, è importante non limitarsi alla pubblicazione di un documento di specifica ma **garantire una pubblicazione sul Web in formato aperto, machine-readable e possibilmente attraverso l’adozione di standard**, con l’uso di URI (Uniform Resource Identifier) persistenti e deferenziabili e con l’associazione di una licenza aperta che ne consenta il massimo riutilizzo.

Questo approccio, seguito ampiamente nella definizione dell’ontologia DCAT-AP_IT, consente di:

 + massimizzare il riutilizzo dell’ontologia stessa, anche in altri contesti;
 + collegare l’ontologia ad altre già presenti nel web dei dati. Per esempio, lo sviluppo OWL  dell’ontologia DCAT-AP_IT ha consentito di collegarla all’ontologia OWL del profilo CPSV-AP_IT abilitando così un collegamento tra dati e servizi;
 + porre le basi per la costruzione di applicazioni avanzate che utilizzano l’ontologia. Ne sono un esempio anche i meccanismi automatici di harvesting verso altri portali (e.g., portale europeo dei dati);
 + porre le basi per garantire interoperabilità semantica anche nella definizione di metadati descrittivi di dati e di cataloghi delle pubbliche amministrazioni.

A questo va aggiunto che è altresì importante garantire che l’ontologia sia facilmente comprensibile da persone e non solo da software. A tal proposito, è cruciale fornire:

 + un’ontologia OWL dove le etichette, assegnate alle varie proprietà e classi, e i commenti siano in più lingue (così l’ontologia OWL DCAT-AP_IT è espressa sia in italiano che in inglese);
 + strumenti che consentano di navigare facilmente l’ontologia attraverso il Web. A tale proposito l’ontologia OWL di DCAT-AP_IT può essere acceduta e consultata mediante strumenti quali LODE (DCAT-AP_IT è navigabile via LODE in `italiano <http://www.essepuntato.it/lode/owlapi/lang=it/http://www.dati.gov.it/onto/dcatapit>`__ e in `inglese <http://www.essepuntato.it/lode/owlapi/lang=en/http://www.dati.gov.it/onto/dcatapit>`__) e WebVOWL (`DCAT-AP_IT ha una rappresentazione grafica <http://www.dati.gov.it/webvowl/#dcatapit>`__).
