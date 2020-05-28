<p align="center">
<a href="https://extendedicons.vigonotion.com/">
<img src="images/logo.svg" alt="Extended Icons" width=64 height=64>
</a>
<h3 align="center">Extended Icons</h3>
<p align="center">
Some not so popular icons that are out of scope of the great <a href="https://simpleicons.org">SimpleIcons.org</a> project.
</p>

<p align="center">
You can view them on <a href="https://extendedicons.vigonotion.com">extendedicons.vigonotion.com</a>.
</p>
</p>

## About Extended Icons and it's relation to Simple Icons

I created this repository because some icons I need for my project are out of scope
for the simple icons project. These include icons that have a low Alexa rank or
only have local relevance. Yet I really love the simple icons infrastructure, so
I based this repository on their work. This repository will **only ever** contain
icons that are out of scope of simple icons, and shall be **an extension to the project,
not a competitive or alternative**.


## Usage

### General Usage

Icons can be downloaded as SVGs directly from [our website](https://extendedicons.vigonotion.com/) - simply click the icon you want, and the download should start automatically.

### CDN Usage

Icons can be served from a CDN such as [JSDelivr](https://www.jsdelivr.com/package/npm/extended-icons) or [Unpkg](https://unpkg.com/browse/extended-icons/). Simply use the `extended-icons` npm package and specify a version in the URL like the following:

```html
<img height="32" width="32" src="https://cdn.jsdelivr.net/npm/extended-icons@v2/icons/[ICON NAME].svg" />
<img height="32" width="32" src="https://unpkg.com/extended-icons@v2/icons/[ICON NAME].svg" />
```

Where `[ICON NAME]` is replaced by the icon name, for example:

```html
<img height="32" width="32" src="https://cdn.jsdelivr.net/npm/extended-icons@v2/icons/extendedicons.svg" />
<img height="32" width="32" src="https://unpkg.com/extended-icons@v2/icons/extendedicons.svg" />
```

These examples use the latest major version. This means you won't receive any updates following the next major release. You can use `@latest` instead to receive updates indefinitely. However, this will result in a `404` error if the icon is removed.

### Node Usage

The icons are also available through our npm package. To install, simply run:

```
$ npm install extended-icons
```

The API can then be used as follows:

```javascript
const extendedIcons = require('extended-icons');

console.log(extendedIcons.get('Extended Icons'));

/*
{
    title: 'Extended Icons',
    slug: 'extendedicons',
    hex: '111111',
    source: 'https://extendedicons.vigonotion.com/',
    svg: '<svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">...</svg>',
    path: 'M12 12v-1.5c-2.484 ...'
}
*/
```

Alternatively you can import the needed icons individually.
This is useful if you are e.g. compiling your code with [webpack](https://webpack.js.org/) and therefore have to be mindful of your package size:

```javascript
const icon = require('extended-icons/icons/extendedicons');

console.log(icon);

/*
{
    title: 'Extended Icons',
    slug: 'extendedicons',
    hex: '111111',
    source: 'https://extendedicons.vigonotion.com/',
    svg: '<svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">...</svg>',
    path: 'M12 12v-1.5c-2.484 ...'
}
*/
```

#### TypeScript Usage

There are also TypeScript type definitions for the Node package. To use them, simply run:

```
$ npm install @types/extended-icons
```

### PHP Usage

The icons are also available through our Packagist package. To install, simply run:

```
$ composer require extended-icons/extended-icons
```

The package can then be used as follows:

```php
<?php

echo file_get_contents('path/to/package/icons/extended-icons.svg');

// <svg role="img" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">...</svg>
?>
```

## Status

[![Build Status](https://travis-ci.com/extended-icons/extended-icons.svg?branch=develop)](https://travis-ci.com/extended-icons/extended-icons)
[![npm version](https://img.shields.io/npm/v/extended-icons.svg)](https://www.npmjs.com/package/extended-icons)
[![Packagist version](https://img.shields.io/packagist/v/extended-icons/extended-icons)](https://packagist.org/packages/extended-icons/extended-icons)
