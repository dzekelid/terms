swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 1
info:
  title: AWS Service Catalog API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=TerminateProvisionedProduct:
    get:
      summary: Terminate Provisioned Product
      description: Requests termination of an existing ProvisionedProduct object.
      operationId: terminateProvisionedProduct
      x-api-path-slug: actionterminateprovisionedproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: IgnoreErrors
        description: If set to true, AWS Service Catalog stops managing the specified
          ProvisionedProduct object even         if it cannot delete the underlying
          resources
        type: string
      - in: query
        name: ProvisionedProductId
        description: The identifier of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: ProvisionedProductName
        description: The name of the ProvisionedProduct object to terminate
        type: string
      - in: query
        name: TerminateToken
        description: An idempotency token that uniquely identifies the termination
          request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Provisioned Products