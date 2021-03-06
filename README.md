react-precache-img [![npm](https://img.shields.io/npm/dt/react-precache-img.svg)]() [![npm](https://img.shields.io/npm/v/react-precache-img.svg)](https://www.npmjs.com/package/react-precache-img) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/mcarlucci/react-precache-img/blob/master/LICENSE)
================

> React component that pre-caches images in the browser

Key features:

- Preload a list of images in the browser for immediate use later in a user session
- Does not render any actual HTML DOM elements, making it non-intrusive
- Extremely lightweight at under 1kb

Install
-------

```bash
npm install --save react-precache-img
```

Usage
-------

```js
import React from 'react';
import PreCacheImg from 'react-precache-img';

return (
    <PreCacheImg
      images={[
        'http://searchengineland.com/figz/wp-content/seloads/2015/12/google-amp-fast-speed-travel-ss-1920.jpg',
        'https://upload.wikimedia.org/wikipedia/commons/6/62/Starsinthesky.jpg'
      ]}
    />
);
```
#### Testing:
In Chrome, clear your browser cache, then copy and paste this in a new tab to view your cache: `chrome://cache/`

After you load a page with the above example component, you should see http://searchengineland.com/figz/wp-content/seloads/2015/12/google-amp-fast-speed-travel-ss-1920.jpg and https://upload.wikimedia.org/wikipedia/commons/6/62/Starsinthesky.jpg at the top of the list.

Props
---
#### `images={[Array]} [required]`

List of image URLs/URIs to be pre-cached
