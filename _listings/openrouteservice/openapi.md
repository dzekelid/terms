---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
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
---