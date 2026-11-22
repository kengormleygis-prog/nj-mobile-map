# README – Standalone qgis2web Export

This export is completely "self-contained".

To view the map, simply open "index.html" by double-clicking it.
No web server or additional software is required.

The map works because all the required JavaScript libraries are included
in the export. The application loads the GeoJSON layer data and their styles
directly from the local files. Stormwater basin locations, inlets, and power
plants can be toggled from the layer control in the upper-right corner. Use
the address search above the map to find New Jersey locations.
Tap the location button to request a one-time device location; the browser
will ask for permission. Location is not stored, and this feature requires
HTTPS or localhost.
Open any map point and choose "Drive here in Google Maps" to get directions.

## QGIS Source Project

The original QGIS project and its GeoJSON data are in the "qgis-project"
folder. Open "qgis-project/nj_test.qgz" in QGIS; its data paths are relative
so the project works after cloning or downloading this repository.

## Publishing on a Website

If you upload the entire folder to a web server, the map will work 
immediately by opening the "index.html" file.

Example:

"https://www.example.com/my-map/index.html"

## Publishing with GitHub Pages

Push this entire folder to a GitHub repository. In the repository settings,
open Pages and set Source to "GitHub Actions". The included workflow publishes
the repository's root directory as the mobile-friendly website.
