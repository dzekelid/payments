---
swagger: "2.0"
x-collection-name: PayPal
x-complete: 0
info:
  title: Paypal Update Invoice
  description: Use the UpdateInvoice API operation to update an invoice.
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Permissions/GetAdvancedPersonalData:
    post:
      summary: Get Advanced Personal Data
      description: Use the GetAdvancedPersonalData API operation to obtain sensitive
        personal data for an account holder.
      operationId: Permissions.GetAdvancedPersonalData.post
      x-api-path-slug: permissionsgetadvancedpersonaldata-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Profiles
  /Permissions/GetBasicPersonalData:
    post:
      summary: Get Basic Personal Data
      description: Use the GetBasicPersonalData API operation to obtain basic personal
        data for an account holder.
      operationId: Permissions.GetBasicPersonalData.post
      x-api-path-slug: permissionsgetbasicpersonaldata-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Profiles
  /Permissions/CancelPermissions:
    post:
      summary: Cancel Permissions
      description: Use the CancelPermissions API operation to cancel access to a set
        of permissions.
      operationId: Permissions.CancelPermissions.post
      x-api-path-slug: permissionscancelpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Permissions/GetPermissions:
    post:
      summary: Get Permissions
      description: Use the GetPermissons API operation to obtain the permissions associated
        with an access token.
      operationId: Permissions.GetPermissions.post
      x-api-path-slug: permissionsgetpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Permissions/GetAccessToken:
    post:
      summary: GetAccess Token
      description: Use the GetAccessToken API operation to obtain an access token
        for a set of permissions.
      operationId: Permissions.GetAccessToken.post
      x-api-path-slug: permissionsgetaccesstoken-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Access Tokens
  /Permissions/RequestPermissions:
    post:
      summary: Request Permissions
      description: "Use the RequestPermissions API operation to request permissions
        to execute API operations on a PayPal account holder\u2019s behalf."
      operationId: Permissions.RequestPermissions.post
      x-api-path-slug: permissionsrequestpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Invoice/SearchInvoices:
    post:
      summary: Search Invoices
      description: Use the SearchInvoice API operation to search an invoice.
      operationId: Invoice.SearchInvoices.post
      x-api-path-slug: invoicesearchinvoices-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
      - Search
  /Invoice/MarkInvoiceAsPaid:
    post:
      summary: Mark Invoice As Paid
      description: Use the MarkInvoiceAsPaid API operation to mark an invoice as paid.
      operationId: Invoice.MarkInvoiceAsPaid.post
      x-api-path-slug: invoicemarkinvoiceaspaid-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/Cancel Invoice:
    post:
      summary: Cancel Invoice
      description: Use the CancelInvoice API operation to cancel an invoice.
      operationId: Invoice.CancelInvoice.post
      x-api-path-slug: invoicecancel-invoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/GetInvoiceDetails:
    post:
      summary: Get Invoice Details
      description: Use the GetInvoiceDetails API operation to get detailed information
        about an invoice.
      operationId: Invoice.GetInvoiceDetails.post
      x-api-path-slug: invoicegetinvoicedetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/UpdateInvoice:
    post:
      summary: Update Invoice
      description: Use the UpdateInvoice API operation to update an invoice.
      operationId: Invoice.UpdateInvoice.post
      x-api-path-slug: invoiceupdateinvoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
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