---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Gets accounting system balance
  version: 1.0.0
  description: Gets accounting system balance.
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