Google Maps V3 Marker Clusterer
==============================
This is a fork of Xiaoxi Wu's MarkerClusterer library for Google Maps V3.

The original repository can be found here: http://google-maps-utility-library-v3.googlecode.com/svn/trunk/markerclusterer/

**NOTE:** I will likely only be editing `src/markerclusterer.js`, since that's really the only part I care about. The docs, examples, images, and compiled version all came along when I forked from the original SVN repository.

Added Features
--------------

* Support for `offsetX` and `offsetY` style options that can be used to make cluster icons off-center. Useful if you want a pin-shaped cluster marker, for example.
* Support a negative value for the X `anchor`. This adds padding-right instead of padding-left, in order to cut back the area labels can use on the right side instead of the left side.
* Support for `textAlign` style option, that takes `left`, `center`, `right`, to override the default value used by the library. Useful with a negative X anchor for right-justification.
* Support for `fontFamily` style option that allows you to style the text label with a different font.
* Support for `fontWeight` style option that allows you to override the default bold text label.
* Don't re-center the map on the clicked cluster if the map is already at maximum zoom and not performing any additional zoom-in.

