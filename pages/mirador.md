---
layout: page
title: Mirador Viewer
permalink: /mirador/
---



<script src="https://unpkg.com/mirador@latest/dist/mirador.min.js"></script>


  <!-- By default uses Roboto font. Be sure to load this or change the font -->
  <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto:300,400,500">
  <!-- Container element of Mirador whose id should be passed to the instantiating call as "id" -->
  <div id="my-mirador"/> 

  <script type="text/javascript">
  var mirador = Mirador.viewer({
    "id": "my-mirador",
    "manifests": {
      "{{ '/' | absolute_url }}img/derivatives/iiif/f003/manifest.json": {
        "provider": ""}
    },
    "windows": [
      {
        "loadedManifest": "{{ '/' | absolute_url }}img/derivatives/iiif/f003/manifest.json",
        "canvasIndex": 2,
        "thumbnailNavigationPosition": 'far-bottom'
      }
    ]
  }
  );
  </script>

  