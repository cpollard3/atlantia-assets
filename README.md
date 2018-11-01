### Atlantia Assets

This repository houses the static assets used in [atlantia.tv](http://atlanta.tv).

Users are encouraged to submit assets if they follow the current style, have a relatively low triangle count, and fall under either the Public Domain, CC0, CC-BY, or CC-BY-SA license.

##### Workflow for adding new asset

1. Create or modify a Blender file adding the new asset. One unit of measurement in Blender corresponds to approximately one foot in [atlantia.tv](http://atlantia.tv)
2. Export this object from Blender to Three.js JSON format using precision 3. This can be done with the Blender exporter found [here](https://github.com/mrdoob/three.js/tree/dev/utils/exporters/blender). Include vertices, faces, and UVs.
3. The texture map should be generated from an SVG file. To make the colors configurable by a user, assign a group or shape an ID.
4. Modify representation.json adding your new object. Specify its name, configurable SVG IDs, and author following the conventions already in the file. If its an entirely new object, add its location in the library browser.
5. Open index.html in a web browser and make sure your object was was added as intended.
6. Submit a pull request!
