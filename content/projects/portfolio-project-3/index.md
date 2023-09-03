---
title: Portfolio Payment Gateway for WooCommerce
seo_title: Portfolio Payment Gateway For WooCommerce using $XNB
summary: Payment Gateway For WooCommerce using $XNB
description: Payment Gateway For WooCommerce using $XNB Payment validation done through either xeonbit-wallet-rpc or the blockchain explorer.
slug: portfolio-project-paymentp-gateway
author: Richard D.

draft: false
date: 2023-02-20T03:52:30-05:00
lastmod: 
expiryDate: 
publishDate: 

feature_image: 
feature_image_alt: 

project types: 
    - Open Source

techstack:
    - Payment Gateway
    - PHP/CSS
    - JavaScript
live_url: #
source_url: https://github.com/xeonbit-project/xeonbitwp
---

### Features

  * Payment validation done through either xeonbit-wallet-rpc or the explorer.xeonbit.com blockchain explorer.
  * Validates payments with cron, so does not require users to stay on the order confirmation page for their order to validate.
  * Order status updates are done through AJAX instead of Javascript page reloads.
  * Customers can pay with multiple transactions and are notified as soon as transactions hit the mempool.
  * Configurable block confirmations, from 0 for zero confirm to 60 for high ticket purchases.
  * Live price updates every minute; total amount due is locked in after the order is placed for a configurable amount of time (default 60 minutes) so the price does not change after order has been made.
  * Hooks into emails, order confirmation page, customer order history page, and admin order details page.
  * View all payments received to your wallet with links to the blockchain explorer and associated orders.
  * Optionally display all prices on your store in terms of Xeonbit.
  * Shortcodes! Display exchange rates in numerous currencies.
