---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 0
info:
  title: AP Metadata Services Deprecated Terms
  description: Returns a list of deprecated AP vocabulary terms in the specified format
    for the AP Company authority  or for the other four AP authorities.
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  d/DeprecatedTerm.{format}:
    get:
      summary: Deprecated Terms
      description: Returns a list of deprecated AP vocabulary terms in the specified
        format for the AP Company authority  or for the other four AP authorities.
      operationId: getDDeprecatedterm.Format
      x-api-path-slug: ddeprecatedterm-format-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      - in: path
        name: format
        description: The format of the returned taxonomy data (RDF/XML, RDF/TTL or  NewsML-G2)
      responses:
        200:
          description: OK
      tags:
      - Deprecated
      - Terms
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