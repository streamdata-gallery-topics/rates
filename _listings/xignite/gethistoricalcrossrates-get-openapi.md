---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Currencies Get Historical Cross Rates
  description: Returns multiple cross-rates as of a historical date.
  version: 1.0.0
host: www.xignite.com/xCurrencies.json
basePath: /XigniteCurrencies
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListOfficialRates:
    get:
      summary: List Official Rates
      description: List supported official rates.
      operationId: postListofficialrates
      x-api-path-slug: listofficialrates-get
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
      - List
      - Official
      - Rates
  /GetLatestCrossRates:
    get:
      summary: Get Latest Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetlatestcrossrates
      x-api-path-slug: getlatestcrossrates-get
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
      - Latest
      - Cross
      - Rates
  /GetRawCrossRates:
    get:
      summary: Get Raw Cross Rates
      description: Returns a real-time currency cross-rate.
      operationId: postGetrawcrossrates
      x-api-path-slug: getrawcrossrates-get
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
      - Raw
      - Cross
      - Rates
  /GetRealTimeCrossRates:
    get:
      summary: Get Real Time Cross Rates
      description: Returns the latest possible cross rate.
      operationId: postGetrealtimecrossrates
      x-api-path-slug: getrealtimecrossrates-get
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
      - Real
      - Time
      - Cross
      - Rates
  /GetAllCrossRatesForACurrency:
    get:
      summary: Get All Cross Rates For A Currency
      description: Returns all valid cross rates for a currency.
      operationId: postGetallcrossratesforacurrency
      x-api-path-slug: getallcrossratesforacurrency-get
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
      - Cross
      - Rates
      - Currency
  /GetHistoricalCrossRates:
    get:
      summary: Get Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGethistoricalcrossrates
      x-api-path-slug: gethistoricalcrossrates-get
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
      - Historical
      - Cross
      - Rates
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