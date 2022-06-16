## CSP - Whitelisting

HK2 CSP Whitelisting for Magento version 2.3.5 or Above. HK2 CSP Whitelist some of the major url's like Cloudflare, Google Analytics, Google Fonts, Fontawesome, Addthis, Googleapis, Facebook Graph, Pinterest, Vimeo, Twitter, Trust Pilot.

One can disable Magento 2 CSP. However, Disabling results in more possibilities of attacks on the Magento store. (CSP) are a powerful tool to mitigate against Cross Site Scripting (XSS) and related attacks.

**Please Note** :- This module Whitelist CSP in Magento Store Frontend.

## Account & Pricing

This is a Open Source - Free to use Module. No charge or any fee is there to use it.

## How to Configure?

You can add a domain to the whitelist for a policy (like script-src, style-src, font-src and others) by updating the **csp_whitelist.xml present** in **/app/code/HK2/Csp/etc/csp_whitelist.xml** . Please only create rules for URLs that you have verified as safe & safe for your Magento Store. Ensure that you use a unique "id" (e.g. the URL) for each entry within its group. Below screenshot describes Policy Name & Description.

![screenshot1](docs/images/screenshot1.png)

## Features

Fully Customizable as per your Store needs. Check How to Configure Section for more details.
Open Source & Free

## Some of the URL Whitelisted

1. Addthis (moatads is a part of Addthis)
2. Cloudflare
3. Facebook Graph
4. Fontawesome
5. Google Analytics, Google Fonts, Gstatic, Google Tag Manager & Googleapis
6. Pinterest
7. Trust Pilot
8. Twitter
9. Vimeo

## Complete List of URL Whitelisted

### scripts-src Whitelisted

```
*.addthis.com
*.googleapis.com
*.cloudflare.com
*.fontawesome.com
*.google.com
*.google-analytics.com
googletagmanager.com
graph.facebook.com
*.gstatic.com
*.moatads.com
*.trustpilot.com
*.vimeo.com
widgets.pinterest.com
```

### style-src Whitelisted

```
*.cloudflare.com
*.fontawesome.com
*.googleapis.com
*.gstatic.com
*.twitter.com
```

### img-src Whitelisted

```
*.cloudflare.com
data:
*.google-analytics.com
*.paypal.com
*.twitter.com
*.vimeocdn.com
```

### connect-src Whitelisted

```
*.cloudflare.com
*.paypal.com
*.twitter.com
```

### font-src Whitelisted

```
*.cloudflare.com
*.fontawesome.com
*.googleapis.com</value>
*.gstatic.com
*.twitter.com
```

### frame-src Whitelisted

```
*.addthis.com
*.google.com
*.trustpilot.com
*.twitter.com
*.vimeo.com
```

## Support:

-   Magento v2.3.5, 2.4.x

## Features

1. Fully Customizable as per your Store needs. Check How to Configure Section for more details.
2. Simple, Open Source & Free
3. CSP is not disabled rather specific listed urls are whitelisted, keeping your Magento Store Safe.

## How to install

### Method 1: Install ready-to-paste package

[Download Link - HK2 - CSP - (https://www.techbasant.in/modules/hk2_csp-1.0.0.zip)](https://www.techbasant.in/modules/hk2_csp-1.0.0.zip 'Link')

Download the zip package and unzip it in app/code folder.

## Enable Extension:

```
php bin/magento module:enable HK2_Csp

php bin/magento setup:upgrade

php bin/magento cache:flush
```

## Disable Extension:

```
php bin/magento module:disable HK2_Csp

php bin/magentosetup:upgrade

php bin/magento cache:flush
```

### Method 2: Install via composer (Recommend)

Run the following command in Magento 2 root folder

```
composer require hk2/csp
php bin/magento setup:upgrade
php bin/magento setup:static-content:deploy
```

## Maintenance mode

You may want to enable the maintenance mode when installing or updating the module, especially when working on a production website. To do so, run the two commands below before and after running the other setup commands:

### Enable Maintenance Mode

```
php bin/magento maintenance:enable
```

### Disable Maintenance Mode

```
php bin/magento maintenance:disable
```

Feel Free to send your suggestions of any changes/improvements, will be happy to add the changes.
