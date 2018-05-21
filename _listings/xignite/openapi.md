---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Global Indices Real Time
  description: this-web-service-provides-global-real-time-information-for-us-and-international-indices
  version: 1.0.0
host: globalindicesrealtime.xignite.com
basePath: xglobalindicesrealtime.json/XigniteGlobalIndicesRealTime
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetIndexSymbolMappingsByOldSymbols:
    post:
      summary: Get Index Symbol Mappings By Old Symbols
      description: Get index symbol mappings by old symbols.
      operationId: GetIndexSymbolMappingsByOldSymbols
      x-api-path-slug: getindexsymbolmappingsbyoldsymbols-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Index
      - Symbol
      - Mappings
      - Old
      - Symbols
---