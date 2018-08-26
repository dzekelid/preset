---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/orders/shipping/presets/{presetId}/parcel_service_regions:
    get:
      summary: Lists parcel service regions by parcel service preset id.
      description: Lists parcel service regions. The ID of the parcel service preset
        must be specified.
      operationId: getRestOrdersShippingPresetsPresetParcelServiceRegions
      x-api-path-slug: restordersshippingpresetspresetidparcel-service-regions-get
      parameters:
      - in: query
        name: $parcelServicePresetId
        description: The ID of the parcel service preset
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: presetId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Parcel
      - Service
      - Regions
      - By
      - Parcel
      - Service
      - Preset
      - Id
---