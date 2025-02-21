# @turf/sample

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## sample

Takes a [FeatureCollection][1] and returns a FeatureCollection with given number of [features][2] at random.

### Parameters

*   `featurecollection` **[FeatureCollection][3]** set of input features
*   `num` **[number][4]** number of features to select

### Examples

```javascript
var points = turf.randomPoint(100, {bbox: [-80, 30, -60, 60]});

var sample = turf.sample(points, 5);

//addToMap
var addToMap = [points, sample]
turf.featureEach(sample, function (currentFeature) {
  currentFeature.properties['marker-size'] = 'large';
  currentFeature.properties['marker-color'] = '#000';
});
```

Returns **[FeatureCollection][3]** a FeatureCollection with `n` features

[1]: https://tools.ietf.org/html/rfc7946#section-3.3

[2]: https://tools.ietf.org/html/rfc7946#section-3.2

[3]: https://tools.ietf.org/html/rfc7946#section-3.3

[4]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

<!-- This file is automatically generated. Please don't edit it directly:
if you find an error, edit the source file (likely index.js), and re-run
./scripts/generate-readmes in the turf project. -->

---

This module is part of the [Turfjs project](http://turfjs.org/), an open source
module collection dedicated to geographic algorithms. It is maintained in the
[Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create
PRs and issues.

### Installation

Install this module individually:

```sh
$ npm install @turf/sample
```

Or install the Turf module that includes it as a function:

```sh
$ npm install @turf/turf
```
