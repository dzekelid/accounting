---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get a VAT configuration for the standard accounting location
    of a client
  description: Gets the VAT configuration currently used for the country of the standard
    accounting location of a client (store). The ID of the client (store) must be
    specified.
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
  /rest/accounting/locations:
    post:
      summary: Create an accounting location
      description: Creates an accounting location for a client. The plenty ID of the
        client must be specified.
      operationId: postRestAccountingLocations
      x-api-path-slug: restaccountinglocations-post
      parameters:
      - in: body
        name: /rest/accounting/locations
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}:
    delete:
      summary: Delete an accounting location
      description: Deletes an accounting location. The ID of the accounting location
        must be specified. Standard accounting locations can not be deleted.
      operationId: deleteRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-delete
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
    get:
      summary: Get an accounting location
      description: Gets an accounting location. The ID of the accounting location
        must be specified.
      operationId: getRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
    put:
      summary: Update an accounting location
      description: Updates an accounting location. The ID of the accounting location
        must be specified.
      operationId: putRestAccountingLocationsLocation
      x-api-path-slug: restaccountinglocationslocationid-put
      parameters:
      - in: body
        name: /rest/accounting/locations/{locationId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/debtor_account_configurations:
    get:
      summary: Get debtor account configuration of an accounting location
      description: Gets the debtor account configuration of an accounting location.
        The ID of the accounting location has to be specified. The debtor account
        configuration can contain one standard debtor account only or e.g. several
        accounts for each country of delivery.
      operationId: getRestAccountingLocationsLocationDebtorAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationiddebtor-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Debtor
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/posting_key_configurations:
    get:
      summary: Get a posting key configuration of an accounting location
      description: Gets a posting key configuration of an accounting location. The
        ID of the accounting location has to be specified. The posting key configuration
        can contain up to 4 posting keys.
      operationId: getRestAccountingLocationsLocationAddingKeyConfigurations
      x-api-path-slug: restaccountinglocationslocationidposting-key-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Posting
      - Key
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/locations/{locationId}/revenue_account_configurations:
    get:
      summary: Get the revenue account configuration of an accounting location
      description: Gets the revenue account configuration of an accounting location.
        A revenue account location configuration contains several revenue accounts.
        The ID of the accounting location has to be specified.
      operationId: getRestAccountingLocationsLocationRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationslocationidrevenue-account-configurations-get
      parameters:
      - in: path
        name: locationId
      responses:
        200:
          description: OK
      tags:
      - Revenue
      - Account
      - Configuration
      - Of
      - Accounting
      - Location
  /rest/accounting/stores/locations:
    get:
      summary: List all accounting locations
      description: List all accounting locations.
      operationId: getRestAccountingStoresLocations
      x-api-path-slug: restaccountingstoreslocations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Accounting
      - Locations
  /rest/accounting/stores/{plentyId}/locations:
    get:
      summary: List accounting locations of a client
      description: Lists accounting locations of a client. The plenty ID of the client
        must be specified.
      operationId: getRestAccountingStoresPlentyLocations
      x-api-path-slug: restaccountingstoresplentyidlocations-get
      parameters:
      - in: query
        name: locationId
        description: The plenty ID
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounting
      - Locations
      - Of
      - Client
  /rest/orders/documents/accounting_summary:
    get:
      summary: List document accounting summaries
      description: Lists document accounting summaries. A document accounting summary
        is saved along with each reversal document (for invoice and credit note).
        It contains accounting information about the order for this point in time.
        The summary is saved because an order can be updated after a reversal_document
        is generated. The information about the order before the update is needed
        for accounting.
      operationId: getRestOrdersDocumentsAccountingSummary
      x-api-path-slug: restordersdocumentsaccounting-summary-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: documentType
        description: The document type
      - in: query
        name: itemsPerPage
        description: The number of summaries to be displayed per page
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Accounting
      - Summaries
  /rest/stores/{plentyId}/locations:
    get:
      summary: Get the ID of an accounting location of a country
      description: Gets the ID of an accounting location of a country. The plenty
        ID of the client and the ID of the country must be specified.
      operationId: getRestStoresPlentyLocations
      x-api-path-slug: reststoresplentyidlocations-get
      parameters:
      - in: query
        name: countryId
        description: The ID of the country of the accounting location
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - ID
      - Of
      - Accounting
      - Location
      - Of
      - Country
  /rest/vat/locations/{locationId}:
    get:
      summary: List VAT configurations of an accounting location
      description: Lists the VAT configurations for all countries of one accounting
        location
      operationId: getRestVatLocationsLocation
      x-api-path-slug: restvatlocationslocationid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
      - Of
      - Accounting
      - Location
  /rest/vat/standard:
    get:
      summary: Get a VAT configuration for the standard accounting location of a client
      description: Gets the VAT configuration currently used for the country of the
        standard accounting location of a client (store). The ID of the client (store)
        must be specified.
      operationId: getRestVatStandard
      x-api-path-slug: restvatstandard-get
      parameters:
      - in: query
        name: plentyId
        description: The plenty ID of the client (store)
      - in: query
        name: startedAt
        description: The date in the W3C format when the vat configuration went into
          effect
      responses:
        200:
          description: OK
      tags:
      - VAT
      - Configurationthe
      - Standard
      - Accounting
      - Location
      - Of
      - Client
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