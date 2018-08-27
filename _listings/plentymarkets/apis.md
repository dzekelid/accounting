---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Accounting
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - Create an accounting location
  x-api-slug: restaccountinglocations-post
  description: Creates an accounting location for a client. The plenty ID of the client
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocations-post-openapi.md
- name: plentymarkets REST-API - Delete an accounting location
  x-api-slug: restaccountinglocationslocationid-delete
  description: Deletes an accounting location. The ID of the accounting location must
    be specified. Standard accounting locations can not be deleted.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationid-delete-openapi.md
- name: plentymarkets REST-API - Get an accounting location
  x-api-slug: restaccountinglocationslocationid-get
  description: Gets an accounting location. The ID of the accounting location must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationid-get-openapi.md
- name: plentymarkets REST-API - Update an accounting location
  x-api-slug: restaccountinglocationslocationid-put
  description: Updates an accounting location. The ID of the accounting location must
    be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationid-put-openapi.md
- name: plentymarkets REST-API - Get debtor account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationiddebtor-account-configurations-get
  description: Gets the debtor account configuration of an accounting location. The
    ID of the accounting location has to be specified. The debtor account configuration
    can contain one standard debtor account only or e.g. several accounts for each
    country of delivery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationiddebtor-account-configurations-get-openapi.md
- name: plentymarkets REST-API - Get a posting key configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidposting-key-configurations-get
  description: Gets a posting key configuration of an accounting location. The ID
    of the accounting location has to be specified. The posting key configuration
    can contain up to 4 posting keys.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationidposting-key-configurations-get-openapi.md
- name: plentymarkets REST-API - Get the revenue account configuration of an accounting
    location
  x-api-slug: restaccountinglocationslocationidrevenue-account-configurations-get
  description: Gets the revenue account configuration of an accounting location. A
    revenue account location configuration contains several revenue accounts. The
    ID of the accounting location has to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountinglocationslocationidrevenue-account-configurations-get-openapi.md
- name: plentymarkets REST-API - List all accounting locations
  x-api-slug: restaccountingstoreslocations-get
  description: List all accounting locations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountingstoreslocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountingstoreslocations-get-openapi.md
- name: plentymarkets REST-API - List accounting locations of a client
  x-api-slug: restaccountingstoresplentyidlocations-get
  description: Lists accounting locations of a client. The plenty ID of the client
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountingstoresplentyidlocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restaccountingstoresplentyidlocations-get-openapi.md
- name: plentymarkets REST-API - List document accounting summaries
  x-api-slug: restordersdocumentsaccounting-summary-get
  description: Lists document accounting summaries. A document accounting summary
    is saved along with each reversal document (for invoice and credit note). It contains
    accounting information about the order for this point in time. The summary is
    saved because an order can be updated after a reversal_document is generated.
    The information about the order before the update is needed for accounting.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restordersdocumentsaccounting-summary-get-openapi.md
- name: plentymarkets REST-API - Get the ID of an accounting location of a country
  x-api-slug: reststoresplentyidlocations-get
  description: Gets the ID of an accounting location of a country. The plenty ID of
    the client and the ID of the country must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/reststoresplentyidlocations-get-openapi.md
- name: plentymarkets REST-API - List VAT configurations of an accounting location
  x-api-slug: restvatlocationslocationid-get
  description: Lists the VAT configurations for all countries of one accounting location
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restvatlocationslocationid-get-openapi.md
- name: plentymarkets REST-API - Get a VAT configuration for the standard accounting
    location of a client
  x-api-slug: restvatstandard-get
  description: Gets the VAT configuration currently used for the country of the standard
    accounting location of a client (store). The ID of the client (store) must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/accounting/master/_listings/plentymarkets/restvatstandard-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---