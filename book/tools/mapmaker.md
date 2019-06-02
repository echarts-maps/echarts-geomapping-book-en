# mapmaker

## Introduction

[echarts-mapmaker](https://github.com/echarts-maps/echarts-mapmaker) is derived from
[echarts-map-tool](https://github.com/ecomfe/echarts-map-tool)。mapmaker targets at
echarts map developers, whereas echarts-map-tool is web-ui for downloading
custom geoshapes from Gaode map.

## Installation

```
npm install -g echarts-mapmaker
```


## Feature highlights

### UTF encode geojson

echarts accepts geojson but echarts team invented UTF8-encoded geojson format. UTF8-encoding is a loss compression with its precision adjustable. So far, it is only
used in echarts. Similarly [Topojson](https://github.com/topojson/topojson) is
created and advocated by the king of visualization,
[Mike Bostock](https://github.com/mbostock). Both exists to solve the same
problem: to reduce the size of fat geojson. In the internet era, the user experience
is ruled by response time. The less the payload, the faster the rendering speed.
[For example](https://github.com/echarts-maps/echarts-united-kingdom-js)，the
standard 2017 uk voting map is 188 MB but after UTF8-encoding, the resulting
size is 9.9 MB, 1:20 compression ratio.

## UTF decode geojson

As afore-mentioned, UTF8 encoded geojson can only be used with echarts. Hence,
the decoding facility is required to get standard geojson and echarts-mapmaker provides
such a facility.


Please note: the encoding process is loss comporession

## Simple map authoring: merge and split

mapmaker can merge a geojson feature into another geojson and can split all features
of a geojson file into independent ones.
