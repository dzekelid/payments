---
name: PayPal
x-slug: paypal
description: PayPal is the faster, safer way to send money, make an online payment,
  receive money or set up a merchant account.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
x-kinRank: "10"
x-alexaRank: "71"
tags: Payments
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/apis.md
specificationVersion: "0.14"
apis:
- name: Paypal Get Advanced Personal Data
  x-api-slug: paypal
  description: Use the GetAdvancedPersonalData API operation to obtain sensitive personal
    data for an account holder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/GetAdvancedPersonalData
  tags: Payments,Profiles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionsgetadvancedpersonaldata-post-openapi.md
- name: Paypal Get Basic Personal Data
  x-api-slug: paypal
  description: Use the GetBasicPersonalData API operation to obtain basic personal
    data for an account holder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/GetBasicPersonalData
  tags: Payments,Profiles
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionsgetbasicpersonaldata-post-openapi.md
- name: Paypal Cancel Permissions
  x-api-slug: paypal
  description: Use the CancelPermissions API operation to cancel access to a set of
    permissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/CancelPermissions
  tags: Payments,Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionscancelpermissions-post-openapi.md
- name: Paypal Get Permissions
  x-api-slug: paypal
  description: Use the GetPermissons API operation to obtain the permissions associated
    with an access token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/GetPermissions
  tags: Payments,Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionsgetpermissions-post-openapi.md
- name: Paypal GetAccess Token
  x-api-slug: paypal
  description: Use the GetAccessToken API operation to obtain an access token for
    a set of permissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/GetAccessToken
  tags: Payments,Access Tokens
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionsgetaccesstoken-post-openapi.md
- name: Paypal Request Permissions
  x-api-slug: paypal
  description: "Use the RequestPermissions API operation to request permissions to
    execute API operations on a PayPal account holder\u2019s behalf."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Permissions/RequestPermissions
  tags: Payments,Permissions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/permissionsrequestpermissions-post-openapi.md
- name: Paypal Search Invoices
  x-api-slug: paypal
  description: Use the SearchInvoice API operation to search an invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/SearchInvoices
  tags: Payments,Invoices,Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicesearchinvoices-post-openapi.md
- name: Paypal Mark Invoice As Paid
  x-api-slug: paypal
  description: Use the MarkInvoiceAsPaid API operation to mark an invoice as paid.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/MarkInvoiceAsPaid
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicemarkinvoiceaspaid-post-openapi.md
- name: Paypal Cancel Invoice
  x-api-slug: paypal
  description: Use the CancelInvoice API operation to cancel an invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/Cancel Invoice
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicecancel-invoice-post-openapi.md
- name: Paypal Get Invoice Details
  x-api-slug: paypal
  description: Use the GetInvoiceDetails API operation to get detailed information
    about an invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/GetInvoiceDetails
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicegetinvoicedetails-post-openapi.md
- name: Paypal Update Invoice
  x-api-slug: paypal
  description: Use the UpdateInvoice API operation to update an invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/UpdateInvoice
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoiceupdateinvoice-post-openapi.md
- name: Paypal Create And Send Invoice
  x-api-slug: paypal
  description: Use the CreateAndSendInvoice API operation to create and send an invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/CreateAndSendInvoice
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicecreateandsendinvoice-post-openapi.md
- name: Paypal Send Invoice
  x-api-slug: paypal
  description: Use the SendInvoice API operation to send an invoice to a payer, and
    notify the payer of the pending invoice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/SendInvoice
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicesendinvoice-post-openapi.md
- name: Paypal Create Invoice
  x-api-slug: paypal
  description: Use the CreateInvoice API operation to create a new invoice. The call
    includes merchant, payer, and API caller information, in addition to invoice detail.
    The response to the call contains an invoice ID and URL.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////Invoice/CreateInvoice
  tags: Payments,Invoices
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/invoicecreateinvoice-post-openapi.md
- name: Paypal Get User Agreement
  x-api-slug: paypal
  description: The GetUserAgreement API operation lets you retrieve the user agreement
    for the customer to approve the new PayPal account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/GetUserAgreement
  tags: Payments,Aggreements
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountsgetuseragreement-post-openapi.md
- name: Paypal Get Verified Status
  x-api-slug: paypal
  description: The GetVerifiedStatus API operation lets you check if a PayPal account
    status is verified. A PayPal account gains verified status under a variety of
    circumstances, such as when an account is linked to a verified funding source.
    Verified status serves to indicate a trust relationship. For more information
    about account verified status, refer to PayPal.com.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/GetVerifiedStatus
  tags: Payments,Verified,Status
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountsgetverifiedstatus-post-openapi.md
- name: Paypal Set Funding Source Confirmed
  x-api-slug: paypal
  description: The SetFundingSourceConfirmed API operation lets your application set
    up bank accounts as funding sources for PayPal accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/SetFundingSourceConfirmed
  tags: Payments,Verified,Status
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountssetfundingsourceconfirmed-post-openapi.md
- name: Paypal Add Payment Card
  x-api-slug: paypal
  description: The AddPaymentCard API operation lets your application set up credit
    cards as funding sources for PayPal accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/AddPaymentCard
  tags: Payments,Credit Card
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountsaddpaymentcard-post-openapi.md
- name: Paypal Add Bank Account
  x-api-slug: paypal
  description: The AddBankAccount API operation lets your application set up bank
    accounts as funding sources for PayPal accounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/AddBankAccount
  tags: Payments,Bank Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountsaddbankaccount-post-openapi.md
- name: Paypal Create Account
  x-api-slug: paypal
  description: The CreateAccount API operation enables you to create a PayPal account
    on behalf of a third party.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptiveAccounts/CreateAccount
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptiveaccountscreateaccount-post-openapi.md
- name: Paypal Get Funding Plans
  x-api-slug: paypal
  description: Use the GetFundingPlans API operation to determine the funding sources
    that are available for a specified payment, identified by its key, which takes
    into account the preferences and country of the receiver as well as the payment
    amount. You must be both the sender of the payment and the caller of this API
    operation
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/GetFundingPlans
  tags: Payments,Plans
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsgetfundingplans-post-openapi.md
- name: Paypal Get Shipping Addresses
  x-api-slug: paypal
  description: Use the GetShippingAddresses API operation to obtain the selected shipping
    address. You must have created the payment or preapproval key that identifies
    the account holder whose shipping address you want to obtain, or be the primary
    receiver of the payment or one of the parallel receivers of the payment. The shipping
    address is available only if it was provided during the embedded payment flow.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/GetShippingAddresses
  tags: Payments,Addresses
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsgetshippingaddresses-post-openapi.md
- name: Paypal Execute Payment
  x-api-slug: paypal
  description: The ExecutePayment API operation lets you execute a payment set up
    with the Pay API operation with the actionType CREATE. To pay receivers identified
    in the Pay call, set the pay key from the PayResponse message in the ExecutePaymentRequest
    message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/ExecutePayment
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsexecutepayment-post-openapi.md
- name: Paypal Set Payment Options
  x-api-slug: paypal
  description: "You use the SetPaymentOptions API operation to specify settings for
    a payment of the actionType CREATE. \n\t\t\t\t\tThis actionType is specified in
    the PayRequest message."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/SetPaymentOptions
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentssetpaymentoptions-post-openapi.md
- name: Paypal Get Payment Options
  x-api-slug: paypal
  description: You use the GetPaymentOptions API operation to retrieve the payment
    options passed with the SetPaymentOptionsRequest.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/GetPaymentOptions
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsgetpaymentoptions-post-openapi.md
- name: Paypal Refund
  x-api-slug: paypal
  description: Use the Refund API operation to refund all or part of a payment. You
    can specify the amount of the refund and identify the accounts to receive the
    refund by the payment key or tracking ID, and optionally, by transaction ID or
    the receivers of the original payment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/Refund
  tags: Payments,Refunds
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsrefund-post-openapi.md
- name: Paypal Convert Currency
  x-api-slug: paypal
  description: Use the ConvertCurrency API operation to request the current foreign
    exchange (FX) rate for a specific amount and currency.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/ConvertCurrency
  tags: Payments,Currency
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentsconvertcurrency-post-openapi.md
- name: Paypal Cancel Preapproval
  x-api-slug: paypal
  description: Use the CancelPreapproval API operation to handle the canceling of
    preapprovals. Preapprovals can be canceled regardless of the state they are in,
    such as active, expired, deactivated, and previously canceled.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/CancelPreapproval
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentscancelpreapproval-post-openapi.md
- name: Paypal Preapproval Details
  x-api-slug: paypal
  description: "Use the PreapprovalDetails API operation to obtain information about
    an agreement between you and a sender for making payments on the sender\u2019s
    behalf."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/PreapprovalDetails
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentspreapprovaldetails-post-openapi.md
- name: Paypal Preapproval
  x-api-slug: paypal
  description: "Use the Preapproval API operation to set up an agreement between yourself
    and a sender for making payments on the sender\u2019s behalf. You set up a preapprovals
    for a specific maximum amount over a specific period of time and, optionally,
    by any of the following constraints: the number of payments, a maximum per-payment
    amount, a specific day of the week or the month, and whether or not a PIN is required
    for each payment request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/Preapproval
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentspreapproval-post-openapi.md
- name: Paypal Payment Details
  x-api-slug: paypal
  description: Use the PaymentDetails API operation to obtain information about a
    payment. You can identify the payment by your tracking ID, the PayPal transaction
    ID in an IPN message, or the pay key associated with the payment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/PaymentDetails
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentspaymentdetails-post-openapi.md
- name: Paypal Pay
  x-api-slug: paypal
  description: "Use the Pay API operation to transfer funds from a sender\u2019s PayPal
    account to one or more receivers\u2019 PayPal accounts. You can use the Pay API
    operation to make simple payments, chained payments, or parallel payments; these
    payments can be explicitly approved, preapproved, or implicitly approved."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com////AdaptivePayments/Pay
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/adaptivepaymentspay-post-openapi.md
- name: Paypal
  x-api-slug: paypal
  description: PayPal is the faster, safer way to send money, make an online payment,
    receive money or set up a merchant account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/237-paypal.jpg
  humanURL: https://paypal.com
  baseURL: https://svcs.sandbox.paypal.com//
  tags: Payments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/payments/master/_listings/paypal/openapi.md
x-common:
- type: x-base-url
  url: https://api.paypal.com
- type: x-crunchbase
  url: https://crunchbase.com/organization/paypal
- type: x-crunchbase
  url: http://www.crunchbase.com/company/paypal
- type: x-developer
  url: https://developer.paypal.com/
- type: x-faq
  url: https://developer.paypal.com/docs/faq/
- type: x-getting-started
  url: https://developer.paypal.com/docs/
- type: x-github
  url: https://github.com/paypal
- type: x-playground
  url: https://devtools-paypal.com/hateoas/index.html
- type: x-privacy
  url: https://www.paypal.com/us/cgi-bin/webscr?cmd=p/gen/ua/policy_privacy-outside
- type: x-release-notes
  url: https://developer.paypal.com/docs/release-notes/
- type: x-terms-of-service
  url: https://cms.paypal.com/us/cgi-bin/?cmd=_render-content&content_ID=ua/Legal_Hub_full
- type: x-twitter
  url: https://twitter.com/paypal
- type: x-website
  url: https://paypal.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---