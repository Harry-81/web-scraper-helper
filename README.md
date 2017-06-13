# web-scraper-helper
A tool to test web scraping rules.

# Chrome Extension:

## Description
This started out as a tampermonkey script turned into a chrome extension. The goal of this is to make creating and changing the JSON rules for the Coveo webcrawler faster.

## How to build
- Download/clone git repo
- Turn on developer mode in chrome
- Load unpacked extension
- Find the "chrome_extension" folder in the repo

## How to run
On any webpage, just open the developer tools (Control+Shift+I) and navigate to the "CWC Panel"

## Dependencies
Google Chrome or Chromium

# Tampermonkey Script:

## Description
When you create Web or Sitemap sources in the Coveo platform, you can add Web scraping rules to retrieve or to exclude content from the web pages it will crawl.
This Tampermonkey script helps with testing your web scraper rules.
You will be able to test your rules and verify which metadata will be extracted from the page without having to re-index your source.

## How-to Use

* Import the `misc/Webscraping.user.js` file in your Tampermonkey extension.
* From within the Tampermonkey editor:
  * Edit the `@match` to include the site you are working with
  * Edit the `jsonRules`
  * Save the script
* Reload your site

Once you are happy with your rules, copy and paste the JSON structure from the Tampermonkey editor to your Web source in your [Coveo organization](https://platform.cloud.coveo.com/admin/).

## Dependencies
This tool is a Tampermonkey script. You need to install the [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) extension in your Chrome browser to use it.

