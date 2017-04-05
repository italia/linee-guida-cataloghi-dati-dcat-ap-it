Esempi
======

Esempi d'uso di ``dct:Location`` e ``locn:Geometry``


``JSON-LD``

.. code-block:: json
   :linenos:


    	{
          "@id": "http://dati.gov.it/resource/CoperturaSpaziale/LocalizzazioneStudiMedici_r_liguri:D.658",
          "@type": "dcterms:Location",
          "locn:geometry": {
            "@type": "gsp:gmlLiteral",
            "@value": "<gml:Envelope srsName=\"http://www.opengis.net/def/EPSG/0/4326\"><gml:lowerCorner>7.48820862370018 43.5963597132668</gml:lowerCorner><gml:upperCorner>10.0879518636137 44.849579861466</gml:upperCorner></gml:Envelope>"
          }
      },


``RDF/XML``

.. code-block:: xml
   :linenos:

    <!-- http://dati.gov.it/resource/CoperturaSpaziale/LocalizzazioneLineaCosta -->
    <dct:Location rdf:about="http://dati.gov.it/resource/CoperturaSpaziale/LocalizzazioneLineaCosta_r_liguri:D.658">
        <locn:geometry rdf:datatype="&gsp;gmlLiteral">&lt;gml:Envelope
        srsName=&quot;http://www.opengis.net/def/EPSG/0/4326&quot;&gt;&lt;gml:lowerCorner&gt;7.488208623
        70018 43.5963597132668&lt;/gml:lowerCorner&gt;&lt;gml:upperCorner&gt;10.0879518636137
        44.849579861466&lt;/gml:upperCorner&gt;&lt;/gml:Envelope&gt;</locn:geometry>
    </dct:Location>


``RDF/Turtle``

.. code-block:: turtle
   :linenos:

    <http://dati.gov.it/resource/CoperturaSpaziale/LocalizzazioneLineaCosta_r_liguri:D.658>
        a               dct:Location ;
        locn:geometry   "<gml:Envelope
        srsName=\"http://www.opengis.net/def/EPSG/0/4326\"><gml:lowerCorner>7.48820862370018
        43.5963597132668</gml:lowerCorner><gml:upperCorner>10.0879518636137 44.849579861466</gml:upperCorner></gml:Envelope>"^^gsp:gmlLiteral .
