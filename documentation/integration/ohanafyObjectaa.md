# This File describes the OHanafy objects and fields

## Table: Account

**Description:** This table contains information about accounts, including various details related to keg deposits, account attributes, and related entities.

### Fields

| Field Name                         | Description                                                                                           | Type                      | Relationships                      |
|------------------------------------|-------------------------------------------------------------------------------------------------------|---------------------------|-----------------------------------|
| `ohanafy__X1_2_BBL_Deposits__c`    | This is the sum of the deposits collected for 1/2 BBLs for this customer.                           | Currency (16, 2)          | -                                 |
| `ohanafy__X1_2_BBLs__c`            | This is the number of your 1/2 BBL kegs this customer currently has outstanding.                     | Number (5, 0)             | -                                 |
| `ohanafy__X1_4_BBL_Deposits__c`    | This is the sum of the deposits collected for 1/4 BBLs for this customer.                           | Currency (16, 2)          | -                                 |
| `ohanafy__X1_4_BBLs__c`            | This is the number of your 1/4 BBL kegs this customer has outstanding.                              | Number (5, 0)             | -                                 |
| `ohanafy__X1_6_BBL_Deposits__c`    | This is the sum of the deposits collected for 1/6 BBLs for this customer.                           | Currency (16, 2)          | -                                 |
| `ohanafy__X1_6_BBLs__c`            | This is the number of your 1/6 BBL kegs this customer has outstanding.                              | Number (5, 0)             | -                                 |
| `ohanafy__X20_L_Deposits__c`       | This is the sum of the deposits collected for 20 Liter kegs for this customer.                      | Currency (16, 2)          | -                                 |
| `ohanafy__X20_Ls__c`               | This is the number of 20 Liter kegs this customer has outstanding.                                   | Number (5, 0)             | -                                 |
| `ohanafy__X40_L_Deposits__c`       | This is the sum of the deposits collected for 40 Liter kegs for this customer.                      | Currency (16, 2)          | -                                 |
| `ohanafy__X40_Ls__c`               | This is the number of 40 Liter kegs this customer has outstanding.                                   | Number (5, 0)             | -                                 |
| `ohanafy__X50_L_Deposits__c`       | This is the sum of the deposits collected for 50 Liter kegs for this customer.                      | Currency (16, 2)          | -                                 |
| `ohanafy__X50_Ls__c`               | This is the number of 50 Liter kegs this customer has outstanding.                                   | Number (5, 0)             | -                                 |
| `ohanafy__ABC_License_Expiration_Date__c` | The expiration date of the ABC license for this account.                                          | Date                      | -                                 |
| `Description`                      | A text area for describing the account.                                                               | Textarea (32000)          | -                                 |
| `Fax`                              | The fax number associated with this account.                                                           | Phone (40)                | -                                 |
| `Id`                               | The unique identifier for the account.                                                                 | Id (18)                   | -                                 |
| `Name`                             | The name of the account.                                                                             | Text (255)                | -                                 |
| `Phone`                            | The phone number associated with this account.                                                        | Phone (40)                | -                                 |
| `AccountSource`                    | The source through which the account was acquired.                                                     | Picklist (Advertisement; Employee Referral; External Referral; Partner; Public Relations; Seminar - Internal; Seminar - Partner; Trade Show; Web; Word of mouth; Other) | -                                 |
| `Type`                             | The type of account (e.g., Customer, Supplier, etc.).                                                 | Picklist (Customer; Supplier; Vendor/Service; Distributed Customer; Contract Partner) | -                                 |
| `Active`                           | Indicates whether the account is still active.                                                         | Checkbox                  | -                                 |
| `ohanafy__Contractor_Checkbox__c`  | Select if the Supplier Account is a Contractor.                                                        | Checkbox                  | -                                 |
| `AnnualRevenue`                    | The annual revenue of the account.                                                                     | Currency (18, 0)          | -                                 |
| `ohanafy__Billing_Contact__c`      | Lookup to the contact associated with billing for this account.                                        | Lookup (Contact)          | -                                 |
| `ohanafy__Billing_Contact_Email__c`| The email address of the billing contact.                                                               | Formula (Text)            | `ohanafy__Billing_Contact__r.Email` |
| `BillingGeocodeAccuracy`           | The accuracy of the billing address geocode.                                                             | Picklist (Address; Near Address; Block; Street; Extended Zip; Zip; Neighborhood; City; County; State; Unknown) | -                                 |
| `ohanafy__Billing_Street_Address__c` | The billing street address formatted.                                                                  | Formula (Text)            | `BillingStreet & BR() & BillingCity & ", " & BillingState & " " & BillingPostalCode & BR() & BillingCountry` |
| `ohanafy__BOL_Tax_Type__c`        | The type of tax associated with BOL (Bill of Lading).                                                   | Picklist (Bond to Bond; Export; Tax Paid) | -                                 |
| `ohanafy__Bond_Number__c`          | The bond number associated with this account.                                                           | Text (255)                | -                                 |
| `ohanafy__Child_Account__c`        | Indicates whether this account is a child account.                                                      | Formula (Checkbox)        | `IF(ParentId = '', false, true)` |
| `ohanafy__Classification__c`      | The classification of the account (e.g., GRC, Off-Premises).                                           | Picklist (GRC; Off-Premises) | -                                 |
| `CreatedById`                      | The user who created the account.                                                                       | Lookup (User)             | -                                 |
| `CreatedDate`                      | The date when the account was created.                                                                  | Datetime                  | -                                 |
| `ohanafy__Customer_Number__c`      | An internal customer number for identification or invoicing.                                             | Text (255)                | -                                 |
| `ohanafy__Customer_Priority__c`    | The priority of the customer (e.g., High, Medium, Low).                                                 | Picklist (High; Low; Medium) | -                                 |
| `ohanafy__Customer_Since__c`       | The date when the customer first started.                                                               | Date                      | -                                 |
| `ohanafy__SubType__c`              | The sub-type of customer (e.g., Grocery Store, Hotel).                                                   | Picklist (Grocery Store; Bar/Restaurant; Convenience Store; Bottle Shop; Hotel) | -                                 |
| `Jigsaw`                           | Data.com key for the account.                                                                          | Text (20)                 | -                                 |
| `IsDeleted`                        | Indicates if the account has been deleted.                                                               | Checkbox                  | -                                 |
| `ohanafy__Delivery_Contact__c`     | Lookup to the contact associated with delivery.                                                          | Lookup (Contact)          | -                                 |
| `ohanafy__Delivery_Due_Date__c`    | The due date for delivery.                                                                            | Date                      | -                                 |
| `ohanafy__Delivery_Method__c`      | The method of delivery to this customer.                                                                 | Picklist (Customer Pickup; Delivery; Distributor) | -                                 |
| `ohanafy__Delivery_Pickup_Date__c` | The date when delivery is picked up.                                                                    | Date                      | -                                 |
| `ohanafy__Distributor_Checkbox__c` | Indicates if the account is serviced by a distributor.                                                   | Checkbox                  | -                                 |
| `ohanafy__Distributor__c`          | Lookup to the distributor servicing this account.                                                        | Lookup (Account)          | -                                 |
| `ohanafy__Distributor_Rep__c`      | Lookup to the distributor sales representative.                                                          | Lookup (Contact)          | -                                 |
| `distro_id__c`                     | Unique external ID for the distributor.                                                                  | Text (255)                | -                                 |
| `ohanafy__Division_id__c`          | The division ID for the customer.                                                                       | Formula (Text)            | `$CustomMetadata.ohanafy__Customer_Information__mdt.ohanafy__Test_Brewery_Company.ohanafy__Division_Id__c` |
| `ohanafy__EFT_Customer_ID__c`      | The EFT customer ID for electronic payments.                                                            | Text (255)                | -                                 |
| `ohanafy__EFT_Provider__c`         | The provider for electronic funds transfer.                                                              | Picklist (FinTech; iControl; None) | -                                 |
| `Email__c`                         | The email address associated with the account.                                                           | Text (55)                 | -                                 |
| `NumberOfEmployees`                | The number of employees in the account.                                                                  | Number (18, 0)            | -                                 |
| `AccountNumber`                    | The account number for identification.                                                                   | Text (40)                 | -                                 |
| `ParentId`                         | The parent account for this account.                                                                    | Lookup (Account)          | -                                 |
| `ShippingCity`                     | The city for shipping address.                                                                         | Text (40)                 | -                                 |
| `ShippingCountry`                  | The country for shipping address.                                                                       | Text (40)                 | -                                 |
| `ShippingPostalCode`               | The postal code for shipping address.                                                                    | Text (20)                 | -                                 |
| `ShippingState`                    | The state for shipping address.                                                                         | Text (40)                 | -                                 |
| `ShippingStreet`                   | The street address for shipping.                                                                         | Text (255)                | -                                 |
| `UpdatedById`                      | The user who last updated the account.                                                                    | Lookup (User)             | -                                 |
| `UpdatedDate`                      | The date when the account was last updated.                                                              | Datetime                  | -                                 |

### Relationships

- **Billing Contact:** Refers to the contact associated with billing for this account.
- **Delivery Contact:** Refers to the contact associated with delivery.
- **Distributor:** Refers to the distributor servicing this account.
- **Distributor Rep:** Refers to the distributor sales representative.
- **Parent Account:** Refers to the parent account for this account.
- **Created By:** Refers to the user who created the account.
- **Updated By:** Refers to the user who last updated the account.
