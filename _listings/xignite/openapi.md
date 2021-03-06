swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  Draw, Rate, , Preset:
    get:
      summary: Draw Rate Chart Preset
      description: Draw a standard rate chart for a date range.
      operationId: postDrawratechartpreset
      x-api-path-slug: draw-rate--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Rate
      - Chart
      - Preset
  /DrawYieldCurvePreset:
    get:
      summary: Draw Yield Curve Preset
      description: Draw a yield curve for a rate family.
      operationId: postDrawyieldcurvepreset
      x-api-path-slug: drawyieldcurvepreset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Draw
      - Yield
      - Curve
      - Preset
  Topic, , Preset:
    get:
      summary: Get Topic Chart Preset
      description: Get a preset chart for a topic.
      operationId: postGettopicchartpreset
      x-api-path-slug: topic--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Topic
      - Chart
      - Preset
  Topic, Binary, , Preset:
    get:
      summary: Get Topic Binary Chart Preset
      description: Get time-series and a chart in binary format for a topic.
      operationId: postGettopicbinarychartpreset
      x-api-path-slug: topic-binary--preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Topic
      - Binary
      - Chart
      - Preset
  ', Url, Preset':
    get:
      summary: Get Chart Url Preset
      description: Get chart url for a topic.
      operationId: postGetcharturlpreset
      x-api-path-slug: url-preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Url
      - Preset
  ', Binary, Preset':
    get:
      summary: Get Chart Binary Preset
      description: Get chart in binary format for a topic.
      operationId: postGetchartbinarypreset
      x-api-path-slug: binary-preset-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Chart
      - Binary
      - Preset