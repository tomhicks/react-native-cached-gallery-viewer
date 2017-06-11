An Gallery image viewer
=======================

- Will allow to swipe between images
- Download images from internet and cache them using ImageCache
- Zoom on the images.


Install instructions

```
#install modules
yarn add react-native-cached-gallery-viewer
# or
npm install yarn add react-native-cached-gallery-viewer --save
# then as we depend of react-native-cached-image and therefore in react-native-fetch-blob
RNFB_ANDROID_PERMISSIONS=true react-native link react-native-fetch-blob
```

This module is an updated fork of several projects by [https://github.com/ldn0x7dc](https://github.com/ldn0x7dc) in particular:
- [react-native-gallery](https://github.com/ldn0x7dc/react-native-gallery) 
- [react-native-transformable-image](https://github.com/ldn0x7dc/react-native-transformable-image)
- [react-native-view-transformer](https://github.com/ldn0x7dc/react-native-view-transformer)
- [react-native-view-pager](https://github.com/ldn0x7dc/react-native-view-pager)
- [react-native-gesture-responder](https://github.com/ldn0x7dc/react-native-gesture-responder)
- [react-native-scroller](https://github.com/ldn0x7dc/react-native-scroller)

Advantages are:
- it is compatible with React Native >= 0.45
- There are less dependencies so it is easier to update or change functionality
- Some of the PR in the above mentioned modules are included.
- Uses react-native-cached-image to allow to cache images to disk on iOS and Android
Further work
-----
include a version of [this PR](https://github.com/RealGeeks/react-native-gallery/commit/b31ab42f5c3c2ecb4f9a8e381e89c8d9e87cf458) that is compatible with `react-native-cached-image` 