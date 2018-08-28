---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Statistics Get Chart Url Preset
  description: Get chart url for a topic.
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---