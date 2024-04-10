
# ImageViewer

A simple and easliy styled web component for viewing images🖼.

## Usage
First add the repo as a module.
`git submodule add https://github.com/Skrywerbeer/ImageViewer.git`
Add the component definition.
```
<head>
	...
	<script src="/your/project/ImageViewer/imageViewer.js"></script>
	...
</head>
```
Then where convenient add the component itself to your markup, using the provided
slots to add the controls. Like so.
```
...
<image-viewer>
	<button slot="previous"></button>
	<button slot="next"></button>
	<button slot="close"></button>
</image-viewer>
...
```
The slotted elements are styled as usual. The \<img\> element in the shadow dom 
can be styled using the `image-viewer::part(image)` selector.
