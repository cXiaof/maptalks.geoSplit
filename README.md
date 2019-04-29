# maptalks.geosplit

A tool to split Polygon or Line whith one or more lines.

## Examples

### [DEMO](https://cxiaof.github.io/maptalks.geosplit/demo/index.html)

## Install

-   Install with npm: `npm install maptalks.geosplit`.
-   Install with yarn: `yarn add maptalks.geosplit`.
-   Download from [dist directory](https://github.com/cXiaof/maptalks.geosplit/tree/master/dist).
-   Use unpkg CDN: `https://cdn.jsdelivr.net/npm/maptalks.geosplit/dist/maptalks.geosplit.min.js`

## Usage

As a plugin, `maptalks.geosplit` must be loaded after `maptalks.js` in browsers. You can also use `'import { GeoSplit } from "maptalks.geosplit"` when developing with webpack.

```html
<!-- ... -->
<script src="https://cdn.jsdelivr.net/npm/maptalks.geosplit/dist/maptalks.geosplit.min.js"></script>
<!-- ... -->
```

```javascript
const ms = new maptalks.GeoSplit() // use GeoSplit API, targets is not necessary parameters and if no targets user will choose geometry on the map. Get details in API Reference.
```

## API Reference

```javascript
new maptalks.GeoSplit()
// new maptalks.GeoSplit({ deleteTargets: false })
```

-   options
    -   deleteTargets **boolean** decide if targets lines will be removed, default is true

`split(geometry, targets)` **targets can be one line or lines-array**
`submit(callback)` callback can get two attr, the result and deals which be remove in task
`cancel()`
`remove()`

## Contributing

We welcome any kind of contributions including issue reportings, pull requests, documentation corrections, feature requests and any other helps.

## Develop

The only source file is `index.js`.

It is written in ES6, transpiled by [babel](https://babeljs.io/) and tested with [mocha](https://mochajs.org) and [expect.js](https://github.com/Automattic/expect.js).

### Scripts

-   Install dependencies

```shell
$ npm install
```

-   Watch source changes and generate runnable bundle repeatedly

```shell
$ gulp watch
```

-   Package and generate minified bundles to dist directory

```shell
$ gulp minify
```

-   Lint

```shell
$ npm run lint
```

## More Things

-   [maptalks.autoadsorb](https://github.com/cXiaof/maptalks.autoadsorb/issues)
-   [maptalks.multisuite](https://github.com/cXiaof/maptalks.multisuite/issues)
-   [maptalks.geosplit](https://github.com/cXiaof/maptalks.geosplit/issues)
-   [maptalks.polygonbool](https://github.com/cXiaof/maptalks.polygonbool/issues)
-   [maptalks.geo2img](https://github.com/cXiaof/maptalks.geo2img/issues)
-   [maptalks.control.compass](https://github.com/cXiaof/maptalks.control.compass/issues)
-   [maptalks.autogradual](https://github.com/cXiaof/maptalks.autogradual/issues)
