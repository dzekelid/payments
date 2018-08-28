swagger: "2.0"
x-collection-name: PayJunction
x-complete: 1
info:
  title: PayJunction API Basic
  description: todo-add-description
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
  /smartterminals/{smartTerminaIId}/request-payment:
    post:
      summary: Post Smart Trminals Request Payment
      description: /smartterminals/{smartterminald}/request-payment.
      operationId: SmartterminalsRequestPaymentBySmartTerminaIIdPost
      x-api-path-slug: smartterminalssmartterminaiidrequestpayment-post
      parameters:
      - in: query
        name: amountBase
      - in: formData
        name: invoiceNumber
        description: NumericAn invoice number to include in the transaction details
      - in: formData
        name: showReceiptPrompt
        description: true | falsetrue - Displays the receipt prompt
      - in: path
        name: smartTerminaIId
      - in: query
        name: terminalId
      - in: header
        name: X-PJ-Application-Key
      responses:
        200:
          description: OK
      tags:
      - Smart
      - Trminals
      - Request
      - Payment