# QuickBooks Integration Guide

## Introduction

This guide provides step-by-step instructions on how to integrate QuickBooks with your application. QuickBooks integration allows you to automate accounting tasks, manage invoices, track expenses, and more.

## Prerequisites

Before starting the integration, ensure you have the following:
- A QuickBooks Online account
- Developer access to the QuickBooks API
- Your application's Client ID and Client Secret from the QuickBooks Developer Portal

## Step 1: Set Up Your QuickBooks Developer Account

1. Go to the [QuickBooks Developer Portal](https://developer.intuit.com/).
2. Sign in with your QuickBooks Online account.
3. Navigate to the "My Apps" section and click "Create an App".
4. Fill in the necessary details and select "QuickBooks Online and Payments" as the platform.
5. After creating the app, note down the **Client ID** and **Client Secret**.

## Step 2: Install QuickBooks SDK

Install the QuickBooks SDK for your programming language. For example, if you're using Node.js, you can install the `node-quickbooks` package:

```bash
npm install node-quickbooks
```
## Step 3: Log into Ohanafy

1. Go to salesforce.com
2. login with your ohanafy credentials
3. select mappings between ohanafy and qbo
4. click confirm


## Step 4: Test
1. Create an invoice in Ohanafy
2. It syncs to QBO every 6 hours
3. Check QBO that it synced correctly
4. Get paid

## Mappings
QBO Invoice Fields	-> Ohanafy Fields 	or	Ohanafy Fields	
Customer->	Account.ohanafy__QuickBooks_Customer_ID__c			
Customer email	-> Account.ohanafy__Billing_Contact_Email__c			
BillAddr.Line1	->	Account.Name			
BillAddr.Line2	->	Account.BillingAddress.street			
BillAddr.City	->	Account.BillingAddress.city			
BillAddr.Country	->	Account.BillingAddress.country			
BillAddr.PostalCode	->	Account.BillingAddress.postalCode			
BillAddr.CountrySubDivisionCode	->	Account.BillingAddress.state			
Invoice date	->	Invoice.ohanafy__Invoice_Date__c			
Due date	->	Invoice.ohanafy__Payment_Due_Date__c			
Invoice no.	->	Invoice.Name			
Product/Service	->	Invoice Item.ohanafy__QuickBooks_Item_ID__c	or	Invoice Fee.ohanafy__Accounting_System_ID__c	
Description	->	Invoice Item.ohanafy__Item_Name__c	or	Invoice Fee.ohanafy__Fee_Name__c	
QTY	->	Invoice Item.ohanafy__Quantity__c	or	1	
Rate	->	Invoice Item.ohanafy__Sub_Total__c / Invoice Item.ohanafy__Quantity__c	or	Invoice Fee.ohanafy__Amount__c	
Amount	->	Invoice Item.ohanafy__Sub_Total__c	or	Invoice Fee.ohanafy__Amount__c	
Taxable	 if Invoice Item.ohanafy__Sales_Tax__c > 0			
Class	->	Invoice Item.ohanafy__QuickBooks_Class_ID__c			
Total Tax	->	sum(Invoice Item.ohanafy__Sales_Tax__c)			
Total	->	Invoice.ohanafy__Total_Due__c			
