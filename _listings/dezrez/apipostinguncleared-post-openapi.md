---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get uncleared items in accounting system
  version: 1.0.0
  description: Get uncleared items in accounting system.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/systemaccount:
    get:
      summary: Get System Account for the Accounting System
      description: Get system account for the accounting system.
      operationId: Account_GetSystemAccount
      x-api-path-slug: apiaccountsystemaccount-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - System
      - Accountthe
      - Accounting
      - System
  /api/accountingsystem:
    get:
      summary: Gets accounting system for a legal entity
      description: Gets accounting system for a legal entity.
      operationId: AccountingSystem_Get
      x-api-path-slug: apiaccountingsystem-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Accounting
      - Systema
      - Legal
      - Entity
  /api/accountingsystem/systembalance:
    get:
      summary: Gets accounting system balance
      description: Gets accounting system balance.
      operationId: AccountingSystem_GetSystemBalance
      x-api-path-slug: apiaccountingsystemsystembalance-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Accounting
      - System
      - Balance
    put:
      summary: Archives the accounting system
      description: Archives the accounting system.
      operationId: AccountingSystem_ArchiveSystemByforce
      x-api-path-slug: apiaccountingsystemsystembalance-put
      parameters:
      - in: query
        name: force
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Archives
      - Accounting
      - System
  /api/accountingsystem/taxstatus:
    get:
      summary: Get Tax Status of Accounting System
      description: Get tax status of accounting system.
      operationId: AccountingSystem_GetTaxStatus
      x-api-path-slug: apiaccountingsystemtaxstatus-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tax
      - Status
      - Of
      - Accounting
      - System
  /api/accountingsystem/suspense:
    get:
      summary: Get amount of funds held in suspense account of the accounting system
      description: Get amount of funds held in suspense account of the accounting
        system.
      operationId: AccountingSystem_GetSuspenseFunds
      x-api-path-slug: apiaccountingsystemsuspense-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Amount
      - Of
      - Funds
      - Held
      - In
      - Suspense
      - Account
      - Of
      - Accounting
      - System
  /api/accountingsystem/createofficeaccount:
    post:
      summary: Create an office account for the accounting system
      description: Create an office account for the accounting system.
      operationId: AccountingSystem_CreateOfficeAccountBydataContract
      x-api-path-slug: apiaccountingsystemcreateofficeaccount-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Office
      - Accountthe
      - Accounting
      - System
  /api/accountingsystem/officeaccounts:
    get:
      summary: Get list of office accounts associated with the accounting system
      description: Get list of office accounts associated with the accounting system.
      operationId: AccountingSystem_GetOfficeAccounts
      x-api-path-slug: apiaccountingsystemofficeaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Office
      - Accounts
      - Associated
      - Accounting
      - System
  /api/posting/uncleared:
    post:
      summary: Get uncleared items in accounting system
      description: Get uncleared items in accounting system.
      operationId: Posting_GetUnclearedItemsByunclearedItemsDataContract
      x-api-path-slug: apipostinguncleared-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: unclearedItemsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Uncleared
      - Items
      - In
      - Accounting
      - System
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