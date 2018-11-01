### Atlantia Assets

This repository houses the static assets used in [Atlantia Animation](https://store.steampowered.com/app/949500/Atlantia_Animation/).

Users are encouraged to submit assets if they follow the current style, have a relatively low triangle count, and fall under either the Public Domain, CC0, CC-BY, or CC-BY-SA license.

##### Workflow for adding new asset

1. Create or modify a Blender file adding the new asset. One unit of measurement in Blender corresponds to approximately one foot in [Atlantia Animation](https://store.steampowered.com/app/949500/Atlantia_Animation/)
2. Export this object from Blender to Three.js JSON format using precision 3. This can be done with the Blender exporter found [here](https://github.com/mrdoob/three.js/tree/r82/utils/exporters/blender). Include vertices, faces, and UVs.
3. The texture map should be generated from an SVG file. To make the colors configurable by a user, assign a group or shape an ID.
4. Modify representation.json adding your new object. Specify its name, configurable SVG IDs, and author following the conventions already in the file. If its an entirely new object, add its location in the library browser.
5. Open index.html in a web browser and make sure your object was was added as intended. You may need to serve index.html from a local webserver. A simple way to do that is to run *python -m SimpleHTTPServer 3000* in the same directory as index.html, then visit http://localhost:3000/ in a web browser.
6. Submit a pull request!
