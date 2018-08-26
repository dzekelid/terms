---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ClientTrading/termsOfUse:
    get:
      summary: Get API Clienttrading Termsofuse
      description: Get api clienttrading termsofuse.
      operationId: ApiClientTradingTermsOfUseGet
      x-api-path-slug: apiclienttradingtermsofuse-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Clienttrading
      - Termsofuse
  /api/ClientTrading/termsOfUse/margin/agree:
    post:
      summary: Add API Clienttrading Termsofuse Margin Agree
      description: Add api clienttrading termsofuse margin agree.
      operationId: ApiClientTradingTermsOfUseMarginAgreePost
      x-api-path-slug: apiclienttradingtermsofusemarginagree-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Clienttrading
      - Termsofuse
      - Margin
      - Agree
---