# mapshaper

## Introduction

[mapshaper](https://github.com/mbloch/mapshaper) is written by
[Matthew Bloch](https://github.com/mbloch) using node.js. It can edit
Shapefile, GeoJSON, TopoJSON, CSV etc.

With echarts map editing process, it is mainly used to wipe out internal borders.

## Installation

```
npm install -g mapshaper
```

## The most important command for echarts map editing

```
mapshaper your_shape_with_internal_borders.geojson -dissolve2 -o your_shape_contoure.geojson
```

