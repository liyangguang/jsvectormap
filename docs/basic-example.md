---
title: 'Basic example'
description: The section provides basic examples using diffrent approaches to get started.
menu: Basic example
category: overview
position: 1
---

## Using cli
If you're using `webpack` or something like that you'll need to import the map you want to work with after importing jsvectormap.

**Notice**: We're using `world_merc` map not `world` in examples

```javascript
@import 'jsvectormap'
@import 'jsvectormap/dist/maps/world'

const map = new jsVectorMap({
  selector: '#map',
  map: 'world',
})
```

## Overwrite style
Style was written using `Scss` so you can overwrite the default style using variables without twaeaking it, you may want to take a look at [jsvectormap.scss](https://github.com/themustafaomar/jsvectormap/blob/master/src/scss/jsvectormap.scss) to know about all possiable variables.
```scss
// app.scss

$tooltip-bg-color: #374151;
$tooltip-font-family: 'Inter', sans-serif;
$tooltip-font-size: 0.925rem;

// ...
```

## Manually
Getting start `manually` with simple example.

```html
<link rel="stylesheet" href="dist/css/jsvectormap.min.css" />
<script src="dist/js/jsvectormap.min.js"></script>
<script src="dist/maps/world.js"></script>

<div id="map" style="width: 600px; height: 350px"></div>
```

```js
var map = new jsVectorMap({
  selector: "#map",
  map: "world",
});
```