A gallery image viewer
======================

- Will allow to swipe between images
- Download images from internet and cache them using ImageCache
- Zoom on the images.

Install instructions
--------------------

Install the library:

```
yarn add react-native-cached-gallery-viewer
# or
npm install yarn add react-native-cached-gallery-viewer --save
```

and link native dependencies:

```
# we depend on react-native-cached-image which in turn depends on react-native-fetch-blob
RNFB_ANDROID_PERMISSIONS=true react-native link react-native-fetch-blob
```

This module is an updated fork of several projects by [https://github.com/ldn0x7dc](https://github.com/ldn0x7dc). In particular:

- [react-native-gallery](https://github.com/ldn0x7dc/react-native-gallery) 
- [react-native-transformable-image](https://github.com/ldn0x7dc/react-native-transformable-image)
- [react-native-view-transformer](https://github.com/ldn0x7dc/react-native-view-transformer)
- [react-native-view-pager](https://github.com/ldn0x7dc/react-native-view-pager)
- [react-native-gesture-responder](https://github.com/ldn0x7dc/react-native-gesture-responder)
- [react-native-scroller](https://github.com/ldn0x7dc/react-native-scroller)

Advantages are:

- It is compatible with React Native >= 0.45
- There are few dependencies so it is easier to update or change functionality
- Some of the PR in the above mentioned modules are included.
- Uses react-native-cached-image to allow to cache images to disk on iOS and Android

Further work
------------

- Include a version of [this PR](https://github.com/RealGeeks/react-native-gallery/commit/b31ab42f5c3c2ecb4f9a8e381e89c8d9e87cf458) that is compatible with `react-native-cached-image`
- At this moment this library depends on a forked version of `react-native-cached-image` that has all the outstanding PR for the branch 1.3.x merged but it does not uses 1.4.x as the API has change a lot.