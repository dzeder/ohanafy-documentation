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

## Step 3: Log into Ohanafy

1. Go to salesforce.com
2. login with your ohanafy credentials
3. select mappings between ohanafy and qbo
4. click confirm
