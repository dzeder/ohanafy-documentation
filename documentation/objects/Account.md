label | inlineHelpText | type | relationshipName | picklistValues
--- | --- | --- | --- | ---
Id |  | Id |  | 
IsDeleted |  | Boolean |  | 
MasterRecordId |  | Reference | MasterRecord | 
Name |  | String |  | 
Type |  | Picklist |  | Customer, Supplier, Vendor/Service, Distributed Customer, Contract Partner,
RecordTypeId |  | Reference | RecordType | 
ParentId |  | Reference | Parent | 
BillingStreet |  | Textarea |  | 
BillingCity |  | String |  | 
BillingState |  | String |  | 
BillingPostalCode |  | String |  | 
BillingCountry |  | String |  | 
BillingLatitude |  | Double |  | 
BillingLongitude |  | Double |  | 
BillingGeocodeAccuracy |  | Picklist |  | Address, NearAddress, Block, Street, ExtendedZip, Zip, Neighborhood, City, County, State, Unknown,
BillingAddress |  | Address |  | 
ShippingStreet |  | Textarea |  | 
ShippingCity |  | String |  | 
ShippingState |  | String |  | 
ShippingPostalCode |  | String |  | 
ShippingCountry |  | String |  | 
ShippingLatitude |  | Double |  | 
ShippingLongitude |  | Double |  | 
ShippingGeocodeAccuracy |  | Picklist |  | Address, NearAddress, Block, Street, ExtendedZip, Zip, Neighborhood, City, County, State, Unknown,
ShippingAddress |  | Address |  | 
Phone |  | Phone |  | 
Fax |  | Phone |  | 
Website |  | Url |  | 
PhotoUrl |  | Url |  | 
Industry |  | Picklist |  | Agriculture, Apparel, Banking, Biotechnology, Chemicals, Communications, Construction, Consulting, Education, Electronics, Energy, Engineering, Entertainment, Environmental, Finance, Food & Beverage, Government, Healthcare, Hospitality, Insurance, Machinery, Manufacturing, Media, Not For Profit, Other, Recreation, Retail, Shipping, Technology, Telecommunications, Transportation, Utilities,
AnnualRevenue |  | Currency |  | 
NumberOfEmployees |  | Int |  | 
Description |  | Textarea |  | 
OwnerId |  | Reference | Owner | 
CreatedDate |  | Datetime |  | 
CreatedById |  | Reference | CreatedBy | 
LastModifiedDate |  | Datetime |  | 
LastModifiedById |  | Reference | LastModifiedBy | 
SystemModstamp |  | Datetime |  | 
LastActivityDate |  | Date |  | 
LastViewedDate |  | Datetime |  | 
LastReferencedDate |  | Datetime |  | 
Jigsaw |  | String |  | 
JigsawCompanyId |  | String | JigsawCompany | 
AccountSource |  | Picklist |  | Advertisement, Employee Referral, External Referral, Partner, Public Relations, Seminar - Internal, Seminar - Partner, Trade Show, Web, Word of mouth, Other,
SicDesc |  | String |  | 
ohanafy__Active__c | This field is manually updated to indicate whether your relationship with this particular account is still active. | Boolean |  | 
ohanafy__BOL_Tax_Type__c |  | Picklist |  | Bond to Bond, Export, Tax Paid,
ohanafy__Billing_Contact__c | To impact this field, add the contact associated with billing and check the box on the contact record. This will ensure that you have the most updated contact information here. | Reference | ohanafy__Billing_Contact__r | 
ohanafy__Billing_Street_Address__c |  | String |  | 
ohanafy__Bond_Number__c |  | String |  | 
ohanafy__Child_Account__c |  | Boolean |  | 
ohanafy__Classification__c |  | Picklist |  | GRC, Off-Premises,
ohanafy__Customer_Number__c | If you use an internal "customer number" to identify customers or print on the invoice, enter it here. | String |  | 
ohanafy__Customer_Priority__c | Helps you bucket your customers based on their priority. High value (more revenue) generating customers should get highest priorities of service. | Picklist |  | High, Low, Medium,
ohanafy__Customer_Since__c | Populate this field based on the first order date. Measures the longevity of your customer relationships. | Date |  | 
ohanafy__Delivery_Contact__c | To impact this field, add the contact associated with delivery and check the box on the contact record. This will ensure that you have the most updated contact information here. | Reference | ohanafy__Delivery_Contact__r | 
ohanafy__Delivery_Due_Date__c |  | Date |  | 
ohanafy__Delivery_Method__c | Represents the most common method of delivery to this customer account. | Picklist |  | Customer Pickup, Delivery, Distributor,
ohanafy__Delivery_Pickup_Date__c |  | Date |  | 
ohanafy__Distributor_Rep__c | This is the distributor sales rep associated with this customer account. Helpful to have if customer needs off-schedule orders. Contact should be added to the distributor account record and then associated here with the customers they serve. | Reference | ohanafy__Distributor_Rep__r | 
ohanafy__Distributor__c | If this customer is serviced by a distributor, enter the distributor name here. This helps us know with whom our distributors and customers are interacting. | Reference | ohanafy__Distributor__r | 
ohanafy__EFT_Customer_ID__c | If you process payments thru an Electronic Funds Transfer system like Fintech, enter your customer's EFT Customer Number here. | String |  | 
ohanafy__EFT_Provider__c | If you process payments directly thru an Electronic Funds Transfer provider (like Fintech), please select that provider here. | Picklist |  | FinTech, iControl, None,
ohanafy__Energy_Provider__c | Indicates this vendor is an energy provider | Boolean |  | 
ohanafy__Event_Primary_Contact__c | Primary contact for this account, select from the list of available contacts for this account. | Reference | ohanafy__Event_Primary_Contact__r | 
ohanafy__Federal_Tax_ID__c |  | String |  | 
ohanafy__Invoice_Notes__c |  | Textarea |  | 
ohanafy__Last_Order_Date__c | Date of the last order this customer placed | Date |  | 
ohanafy__Last_Purchase_Order_Date__c | This is populated automatically based on your last purchase order from this supplier. Helps you recognize how often you are ordering. | Date |  | 
ohanafy__Legal_Name__c | This is the legal (corporate name) of this customer. | String |  | 
ohanafy__NumberofLocations__c |  | Double |  | 
ohanafy__Order_Date__c |  | Date |  | 
ohanafy__Parent_Account_Report_Id__c |  | String |  | 
ohanafy__Payment_Terms__c | What are your payment terms with this customer or supplier? | Picklist |  | Due on Receipt, 30 Days, 60 Days, 90 Days, Custom,
ohanafy__Permit_Number__c | This is the permit number provided to the customer for alcohol sales and receipts. Don't change this number without sufficient documentation from the customer. | String |  | 
ohanafy__Pricelist__c | Choose the assigned price list here for this customer. All orders and invoices will use this pricelist to calculate amounts due. | Reference | ohanafy__Pricelist__r | 
ohanafy__Priority__c |  | Picklist |  | Low, Medium, High, Very High,
ohanafy__Rating__c | Rate your experience with this Account here. 1 is the worst experience, 5 is the best. This feeds your star rating and should ultimately indicate to you whether or not you want to continue doing business with this account. | Picklist |  | 1, 2, 3, 4, 5,
ohanafy__SLAExpirationDate__c |  | Date |  | 
ohanafy__SLASerialNumber__c |  | String |  | 
ohanafy__SLA__c |  | Picklist |  | Gold, Silver, Platinum, Bronze,
ohanafy__Sales_Rep__c | Represents the person responsible for comprehensively servicing and selling in this account. | Reference | ohanafy__Sales_Rep__r | 
ohanafy__Shipping_Address__c |  | String |  | 
ohanafy__Special_Instructions__c |  | String |  | 
ohanafy__Stage__c | Indicates the stage in customer lifecycle in which this customer falls. Customers are prospects before we've sold them anything, Customers when we are actively selling them products, and Past Customers when they are no longer actively ordering. | Picklist |  | Prospect, Customer, Supplier, Vendor/Service, Past Customer, Past Supplier, Past Vendor/Service,
ohanafy__State_Tax_ID__c | This is the state issued reseller number for sales tax. | String |  | 
ohanafy__Status_Reason__c |  | String |  | 
ohanafy__Status__c | Indicates the status of this account. If you are no longer ordering from, delivering to, or supplying this account, mark it inactive. | Picklist |  | Active, Credit Hold, Inactive,
ohanafy__Supplier_Item_Types__c | Categorizes the items you generally get from this supplier | Multipicklist |  | Keg Shell, Merchandise, Packaging, Raw Materials, Tap Handle,
ohanafy__Tax_Exempt__c | Indicates whether you charge this customer retail sales tax. | Boolean |  | 
ohanafy__Waive_Item_Deposit__c | Be cautious using this box. If it is checked, this means you won't generate invoices for deposits associated with packaging materials. | Boolean |  | 
ohanafy__X1_2_BBL_Deposits__c | This is the sum of the deposits collected for 1/2 BBLs for this customer. | Currency |  | 
ohanafy__X1_2_BBLs__c | This is the number of your 1/2 BBL kegs this customer currently has outstanding. | Double |  | 
ohanafy__X1_4_BBL_Deposits__c | This is the sum of the deposits collected for 1/4 BBLs for this customer | Currency |  | 
ohanafy__X1_4_BBLs__c | This is the number of your 1/4 BBL kegs this customer has outstanding. | Double |  | 
ohanafy__X1_6_BBL_Deposits__c | This is the sum of the deposits collected for 1/6 BBLs for this customer | Currency |  | 
ohanafy__X1_6_BBLs__c | This is the number of your 1/6 BBL kegs this customer has outstanding. | Double |  | 
ohanafy__Total_Energy_Cost__c | Indicates total spend with this provider for energy use | Currency |  | 
ohanafy__Star_Rating__c |  | String |  | 
ohanafy__Total_Keg_Deposits__c | This is the value of all keg deposits with this customer | Currency |  | 
ohanafy__Total_Kegs__c | This is the total number of your kegs this customer currently has outstanding. | Double |  | 
ohanafy__Key__c |  | String |  | 
ohanafy__of_Routes__c |  | Double |  | 
ohanafy__Region__c |  | String |  | 
ohanafy__Mapping_Key__c |  | String |  | 
ohanafy__ABC_License_Expiration_Date__c |  | Date |  | 
ohanafy__Billing_Contact_Email__c |  | String |  | 
ohanafy__Distributor_Checkbox__c |  | Boolean |  | 
ohanafy__QuickBooks_Customer_ID__c |  | String |  | 
ohanafy__Taproom__c |  | Boolean |  | 
ohanafy__Vendor_ABC_Number__c |  | Picklist |  | 123456789,
ohanafy__Division_id__c |  | String |  | 
ohanafy__Payment_Method__c |  | Picklist |  | Check, Cash, EFT, Quickbooks Electronic Invoice,
maps__AssignmentRule__c |  | Reference | maps__AssignmentRule__r | 
ohanafy__Contractor_Checkbox__c | Select if the Supplier Account is a Contractor. | Boolean |  | 
ohanafy__Sub_Type__c |  | Picklist |  | Grocery Store, Convenience Store, Restaurant/Bar, Hotel, Bottle Shop,
ohanafy__Fulfilled_From__c | Select the default order fulfillment location for this customer. | Reference | ohanafy__Fulfilled_From__r | 
Email__c |  | String |  | 
ohanafy__X20_L_Deposits__c |  | Currency |  | 
ohanafy__X20_Ls__c |  | Double |  | 
ohanafy__X40_L_Deposits__c |  | Currency |  | 
ohanafy__X40_Ls__c |  | Double |  | 
ohanafy__X50_L_Deposits__c |  | Currency |  | 
ohanafy__X50_Ls__c |  | Double |  | 
ohanafy__SubType__c | Select the type of customer. | Picklist |  | Grocery Store, Bar/Restaurant, Convenience Store, Bottle Shop, Hotel,
ohanafy__External_ID__c |  | String |  | 
ohanafy__Ohanafy_Master_ID__c |  | String |  | 
Auto_Send_Invoices__c | this is the help | Boolean |  | 
integration_woo_id__c |  | String |  | 
distro_id__c |  | String |  | 
