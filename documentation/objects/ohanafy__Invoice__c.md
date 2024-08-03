ohanafy__Invoice__c

Field Descriptions 
* label: this is the api name of the field used in queries to reference 
* inlineHelpText: the description of what kind of data the field holds 
* type: the data type the field holds 
* relationshipName: this is what is used to query a join to the object in the referenceTo field 
* picklistValues: if the field is a picklist these are the valid options 
* referenceTo: this is the object the relationship refernces 


label | inlineHelpText | type | relationshipName | picklistValues | referenceTo
--- | --- | --- | --- | ---| ---
Id |  | Id |  |  | 
OwnerId |  | Reference | Owner |  | Group
IsDeleted |  | Boolean |  |  | 
Name |  | String |  |  | 
RecordTypeId |  | Reference | RecordType |  | RecordType
CreatedDate |  | Datetime |  |  | 
CreatedById |  | Reference | CreatedBy |  | User
LastModifiedDate |  | Datetime |  |  | 
LastModifiedById |  | Reference | LastModifiedBy |  | User
SystemModstamp |  | Datetime |  |  | 
LastViewedDate |  | Datetime |  |  | 
LastReferencedDate |  | Datetime |  |  | 
ohanafy__Apex_Class_Name__c |  | String |  |  | 
ohanafy__Bill_of_Lading_Number__c |  | String |  |  | 
ohanafy__Customer__c | The customer obligated to this invoice. | Reference | ohanafy__Customer__r |  | Account
ohanafy__Delivery_Pickup_Date__c |  | Date |  |  | 
ohanafy__Delivery__c |  | Reference | ohanafy__Delivery__r |  | ohanafy__Delivery__c
ohanafy__Invoice_Date__c |  | Date |  |  | 
ohanafy__Order__c |  | Reference | ohanafy__Order__r |  | ohanafy__Order__c
ohanafy__Payment_Due_Date__c |  | Date |  |  | 
ohanafy__Reason__c | Primary purpose for this invoice. It is almost always a "Sale". | Picklist |  | Sale, Sample, | 
ohanafy__Sales_Tax_Rate__c |  | Percent |  |  | 
ohanafy__Special_Instructions__c |  | String |  |  | 
ohanafy__Status__c |  | Picklist |  | New, Scheduled, In Progress, Complete, Cancelled, | 
ohanafy__Term__c | Indicates "Payment Terms" on the customer's account record. | Picklist |  | Due on Receipt, 30 Days, 60 Days, 90 Days, Custom, | 
ohanafy__Total_Fees__c |  | Currency |  |  | 
ohanafy__Billing_Contact_Name__c |  | String |  |  | 
ohanafy__Billing_Contact__c | This is the billing contact who has been indicated as such. To update the billing contact, check the box "Billing Contact" on the contact record associated with this customer's billing point of contact. | String |  |  | 
ohanafy__Customer_Name__c |  | String |  |  | 
ohanafy__Customer_Phone__c | Primary phone number of the customer's account. If you need to change this navigate to the customer's account record. | String |  |  | 
ohanafy__Delivery_Contact_Name__c |  | String |  |  | 
ohanafy__Delivery_Contact__c | This is the billing contact who has been indicated as such. To update the billing contact, check the box "Delivery Contact" on the contact record associated with this customer's delivery point of contact. | String |  |  | 
ohanafy__Mailing_Address__c | Populated based on the customer account's primary mailing address. To impact this, update on the customer's account record. | String |  |  | 
ohanafy__Physical_Address_Report__c |  | String |  |  | 
ohanafy__Physical_Address__c |  | String |  |  | 
ohanafy__Reporting_Payment_Due_Date__c | Used for reporting purposes only | Date |  |  | 
ohanafy__Sales_Rep__c | This indicates the sales rep of record on the account or if overridden in the order, the person who placed the order. | String |  |  | 
ohanafy__Total_Due__c | This is the amount collected on the invoice after all credits and returns have been applied. | Currency |  |  | 
ohanafy__Invoice_Revenue__c | This is the revenue generated from product sales on the invoice | Currency |  |  | 
ohanafy__Keg_Credits_Issued__c | Indicates total keg deposit credits issued on this invoice. | Currency |  |  | 
ohanafy__Keg_Deposits_Collected__c | Indicates total keg deposits collected on this invoice. | Currency |  |  | 
ohanafy__Other_Credits_Issued__c | This is the total of credits other than deposits being returned. Examples may include product spoilage or breakage. | Currency |  |  | 
ohanafy__Sales_Tax__c |  | Currency |  |  | 
ohanafy__Sub_Total__c | This is the sum revenue from products sold plus keg deposits collected. This subtotal does not reflect any tax collected nor any credits for returns of kegs or spoilage. | Currency |  |  | 
ohanafy__Payment_Method__c | In what way did this customer pay? | Picklist |  | Check, Cash, EFT, | 
ohanafy__Total_Weight__c |  | Double |  |  | 
ohanafy__Cancelled_Reason__c |  | String |  |  | 
ohanafy__Total_Credits__c |  | Currency |  |  | 
ohanafy__Forms_Mailing_Address_City_State_Zip__c |  | String |  |  | 
ohanafy__Forms_Mailing_Address_Street__c |  | String |  |  | 
ohanafy__Forms_Physical_Address_City_State_Zip__c |  | String |  |  | 
ohanafy__Forms_Physical_Address_Street__c |  | String |  |  | 
ohanafy__Location2__c |  | Reference | ohanafy__Location2__r |  | ohanafy__Location__c
ohanafy__Retail_Alcohol_Sales__c |  | Currency |  |  | 
ohanafy__Retail_Alcohol_Transactions__c |  | Double |  |  | 
ohanafy__Retail_Food_Sales__c |  | Currency |  |  | 
ohanafy__Retail_Food_Transactions__c |  | Double |  |  | 
ohanafy__Retail_Invoice__c |  | Boolean |  |  | 
ohanafy__Retail_Merchandise_Sales__c |  | Currency |  |  | 
ohanafy__Retail_Merchandise_Transactions__c |  | Double |  |  | 
ohanafy__Retail_Misc_Sales__c |  | Currency |  |  | 
ohanafy__Retail_Misc_Transactions__c |  | Double |  |  | 
ohanafy__Retail_Transactions__c |  | Double |  |  | 
ohanafy__Vendor_store_id__c |  | String |  |  | 
ohanafy__invoice_date2__c |  | Date |  |  | 
ohanafy__invoice_due_date__c |  | Date |  |  | 
ohanafy__invoice_number__c |  | String |  |  | 
ohanafy__PO_Number__c |  | String |  |  | 
ohanafy__Po_number_fintech__c |  | String |  |  | 
ohanafy__Retail_Alcohol_Average_Sale__c |  | Currency |  |  | 
ohanafy__Retail_Average_Sale__c |  | Currency |  |  | 
ohanafy__Retail_Food_Average_Sale__c |  | Currency |  |  | 
ohanafy__Retail_Merchandise_Average_Sale__c |  | Currency |  |  | 
ohanafy__Retail_Misc_Average_Sale__c |  | Currency |  |  | 
ohanafy__Retail_Total_Sales__c |  | Currency |  |  | 
ohanafy__Retail_Total_Transactions__c |  | Double |  |  | 
ohanafy__Your_ABC_Permit_Number__c |  | String |  |  | 
Reporting_Invoice_Date__c |  | Date |  |  | 
ohanafy__Date_Month__c |  | Double |  |  | 
Payment_Terms__c |  | String |  |  | 
ohanafy__Integration_Sync_Date__c |  | Datetime |  |  | 
ohanafy__Integration_Sync__c |  | Boolean |  |  | 
ohanafy__gtin_id__c |  | String |  |  | 
ohanafy__po_date__c |  | Date |  |  | 
ohanafy__ref_invoice_number__c |  | String |  |  | 
ohanafy__upc_case__c |  | String |  |  | 
ohanafy__upc_pack__c |  | String |  |  | 
ohanafy__Order_Fulfilled_From__c |  | String |  |  | 
Name_Open_Amt__c |  | String |  |  | 
Kegs_Invoiced__c |  | Double |  |  | 
External_Invoice_Name__c |  | String |  |  | 
integration_accounting_id__c |  | String |  |  | 
integration_accounting_url__c |  | Url |  |  | 
