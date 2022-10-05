---
title: About QR Generator
nav: About
nav_order: 2
---

Library QR Code Generator provides a quick form to generate QR codes for your projects.
QR codes are potentially handy to provide a way for users to open a link on their phone from your print media or display. 

## Usage

The only required field is "Link", the full URL to the page you want to link.
Other fields are optional and should be left blank if you are not using them.

Leave "Image width" blank unless you need a larger PNG for high res print or screens.

"Include I logo" adds U of I logo in center of QR code.

### Tracking via Google Analytics

To add tracking (i.e. a Google [custom campaign](https://support.google.com/analytics/answer/1033863)), please fill in "Tracking campaign id" and "Tracking medium". 
This will automatically add [campaign parameters](https://ga-dev-tools.web.app/ga4/campaign-url-builder/) to the end of the URL that Google Analytics will record when a user follows the link.

- **"Tracking campaign id"** is an identifier for the specific promotion campaign. Use an unique and identifiable name as this will be what we see in Analytics stats.
- **"Tracking medium"** is where you are putting the QR code, such as "poster", "bookmark", "display", or "postcard". 

For example, you might have a single campaign id (e.g. "leganto_launch_2021") where you have several different places you are using a QR code and you want to track useage of each different product (e.g. "postcard", "poster", and "library_screen").
In Analytics we will be able to see total clicks over all for the campaign, plus the distribution of clicks from each source.

To view the stats, you will need access to our Analytics account.

## Why qr-generator?

There are many "free" online platforms for creating QR codes, but some are spammy or risk user privacy.
If a service offers useage statistics or editable URLs, it is not providing clean QR codes, but instead is inserting a tracking short link that your user's traffic is directed through. 
Generally, this is an unnecessary trade off of your user's privacy and data for the slight convienience.
This page provides an open source, non-commercial, client-side, self-hosted alternative (powered by the [QR Code Styling](https://github.com/kozakdenys/qr-code-styling) library).
