# Shopify SanMar Inventory Sync

## Description
This PHP script connects your Shopify store with SanMar's Inventory Service using SOAP and Shopify's Admin API. It fetches products from Shopify, retrieves inventory data from SanMar for each product SKU, and then updates the inventory levels in Shopify accordingly.

## Features
- Fetches product SKUs from Shopify.
- Retrieves current inventory levels from SanMar using SOAP requests.
- Updates the inventory levels in Shopify based on the data retrieved from SanMar.

## Requirements
- **Shopify Store**: A Shopify store with Admin API access.
- **SanMar Credentials**: Valid credentials (`id` and `password`) for accessing the SanMar Inventory Service.
- **SOAP extension**: PHP must have the SOAP extension enabled.
- **cURL extension**: PHP must have the cURL extension enabled.

## Installation
1. **Copy the Script**: Place the PHP script in a secure location on your server.
2. **Dependencies**: Ensure that both the SOAP and cURL PHP extensions are enabled.
3. **Configuration**: Update the script with your Shopify store domain, API access token, location ID, and SanMar credentials.

## Usage
1. **Run the Script**: The script can be executed manually or triggered via a cron job to periodically sync your inventory.
2. **Automation**: Set up a cron job to run the script at your desired frequency.

## Example
Set up a cron job to run this script every hour:
```sh
0 * * * * php /path/to/your/script/opti1shopify.php
