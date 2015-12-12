## ugallery

Uses simple web components to create flexible lightbox2 photo galleries

Dependencies: 
- u-photo.html (components/u-photo.html)
- u-gallery.html (components/u-gallery.html)
- polymer.html (https://github.com/Polymer/polymer)
- webcomnonents-lite.js (https://github.com/webcomponents/webcomponentsjs)
- jquery.min.js (https://jquery.com/)
- lightbox.min.js (https://github.com/lokesh/lightbox2/)
- lightbox.css (https://github.com/lokesh/lightbox2/)

About the u-photo html component:
- creates a gallery image with built-in lightbox features

u-photo options:
- image: string, path to image
- width: string, can be Npx or N%, but % values are recommended (optional; defaults to 100%; NOTE that if a grid value is set on the u-photo or its u-gallery, this value will be overriden)
- album: string, will include this image with others of this album in the lightbox (optional; defaults to "default")
- about: string, shows up as the image caption in lightbox (optional)
- grid: number, determines the image width by setting the number of columns it will occupy (optional)
- cushion: number, sets a padding on the right and left of the image (optional)
- label: boolean, this currently does absolutely nothing, in the future will show/hide lightbox label "image 1 of X"


About the u-gallery html component:
- groups u-photo elements, can size all u-photos it contains into grid
- this can be used solely for grouping & sizing images, or used to display just a cover image that can be clicked to bring up the entire gallery in a lightbox

u-gallery options:
- width: string, can be Npx or N%, but % values are recommended (optional; defaults to 100%)
- album: string, necessary if using cover image & must match album of its u-photos (defaults to "default")
- about: string, shows up as the caption in lightbox (optional)
- cover: string, path to cover image, will enable this feature if value is given (optional)
- grid: number, sets the number of columns in gallery and determines image widths (optional)
- gap: string, can be Npx or N%, sets the space between rows in this gallery (optional; NOTE that this currently breaks the gallery if images aren't all the same size, so use with caution)