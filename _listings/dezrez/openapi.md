swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/account/{id}/paymentoverview:
    post:
      summary: Get payment overview for an account
      description: Get payment overview for an account.
      operationId: Account_GetAccountPaymentOverviewByid
      x-api-path-slug: apiaccountidpaymentoverview-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Overviewan
      - Account
  /api/accounting/exports/batchexport:
    post:
      summary: Get details for batch payment export
      description: Get details for batch payment export.
      operationId: AccountingExport_SetBatchPaymentExportBydataContract
      x-api-path-slug: apiaccountingexportsbatchexport-post
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
      - Detailsbatch
      - Payment
      - Export
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/accounting/exports/batchpaymentcsv:
    post:
      summary: Get details formatted for batch payment csv
      description: Get details formatted for batch payment csv.
      operationId: AccountingExport_ExportBatchPaymentBydataContract
      x-api-path-slug: apiaccountingexportsbatchpaymentcsv-post
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
      - Details
      - Formattedbatch
      - Payment
      - Csv
  /api/progression/lettings/{roleId}/addpayment:
    post:
      summary: Add Tenant Payment
      description: Add tenant payment.
      operationId: LettingsProgression_AddTenantPaymentByroleIdByaddTenantPaymentDataContract
      x-api-path-slug: apiprogressionlettingsroleidaddpayment-post
      parameters:
      - in: body
        name: addTenantPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Tenant
      - Payment
  /api/people/setpaymentdetails:
    put:
      summary: Set the payment details for a person
      description: Set the payment details for a person.
      operationId: People_SetPaymentDetailsBydataContract
      x-api-path-slug: apipeoplesetpaymentdetails-put
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
      - Set
      - Payment
      - Detailsa
      - Person
  /api/people/setprimarypaymentdetails:
    put:
      summary: Set the primary payment details for a person
      description: Set the primary payment details for a person.
      operationId: People_SetPrimaryPaymentDetailsByidByaccountIdBytenantRoleId
      x-api-path-slug: apipeoplesetprimarypaymentdetails-put
      parameters:
      - in: query
        name: accountId
        description: The bank account id
      - in: query
        name: id
        description: The person id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantRoleId
        description: Optional tenant role id to set account as primary
      responses:
        200:
          description: OK
      tags:
      - Set
      - Primary
      - Payment
      - Detailsa
      - Person
  /api/people/removepaymentdetails:
    put:
      summary: Set the payment details for a person
      description: Set the payment details for a person.
      operationId: People_RemovePaymentDetailsByidByaccountId
      x-api-path-slug: apipeopleremovepaymentdetails-put
      parameters:
      - in: query
        name: accountId
        description: The bank account id
      - in: query
        name: id
        description: The person id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Set
      - Payment
      - Detailsa
      - Person
  /api/receipt/recordpayment:
    post:
      summary: Makes payment to supplied account.
      description: Makes payment to supplied account..
      operationId: Receipt_RecordPaymentByrecordPaymentDataContract
      x-api-path-slug: apireceiptrecordpayment-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Makes
      - Payment
      - To
      - Supplied
      - Account
  /api/receipt/paymentitem:
    get:
      summary: Get saved payment items
      description: Get saved payment items.
      operationId: Receipt_GetpaymentItems
      x-api-path-slug: apireceiptpaymentitem-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Payment
      - Items
    put:
      summary: Process payment items
      description: Process payment items.
      operationId: Receipt_ProcessPaymentItems
      x-api-path-slug: apireceiptpaymentitem-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Process
      - Payment
      - Items
    post:
      summary: Saves a payment item to be processed
      description: Saves a payment item to be processed.
      operationId: Receipt_SavePaymentItemByrecordPaymentDataContract
      x-api-path-slug: apireceiptpaymentitem-post
      parameters:
      - in: body
        name: recordPaymentDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Payment
      - Item
      - To
      - Be
      - Processed
    delete:
      summary: Delete a payment item
      description: Delete a payment item.
      operationId: Receipt_DeletePaymentItemByid
      x-api-path-slug: apireceiptpaymentitem-delete
      parameters:
      - in: query
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Payment
      - Item
  /api/receipt/payment/{id}/setexportstatus:
    post:
      summary: Change status export status of payment
      description: Change status export status of payment.
      operationId: Receipt_SetPaymentExportStatusByidBystatusDataContract
      x-api-path-slug: apireceiptpaymentidsetexportstatus-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: statusDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Change
      - Status
      - Export
      - Status
      - Of
      - Payment