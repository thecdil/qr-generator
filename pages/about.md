---
title: About QR Generator
nav: About
nav_order: 2
layout: page-narrow
---

Library QR Code Generator provides a quick form to generate QR codes for your projects.
QR codes are potentially handy to provide a way for users to open a link on their phone from your print media or display. 

## Usage

The only required field is "Link", the full URL to the page you want to link.
Other fields are optional and should be left blank if you are not using them.

Leave "Image width" blank unless you need a larger PNG for high res print or large screens.

Selecting a logo will add the logo image in center of QR code.

### Tracking via Google Analytics

To add tracking (i.e. a Google [custom campaign](https://support.google.com/analytics/answer/11242841)), please fill in "Campaign", "Source", and "Medium" options in the form. 
This will automatically add [campaign parameters](https://support.google.com/analytics/answer/10917952) to the end of the URL that Google Analytics will record when a user follows the link:

- **Campaign (utm_campaign):** the name of the overall marketing campaign (that might have several different sources or mediums). Use a unique and identifiable name as this will be what we see in Analytics stats. E.g. "spec_jazz_2023", "spec_kingspud", "leganto_launch_2021".
- **Source (utm_source):** is the specific referrer that is sending the traffic to the page, identifying the specific item where you are putting the QR code. E.g. "lib-brochure2023", "fye-handout-1", "mill-sticker1".
- **Medium (utm_medium):** is the general marketing medium of the source where you are putting the QR code. E.g. "email", "poster", "bookmark", "sign", or "display".

For example, you might have a single Campaign (e.g. "leganto_launch_2021") where you have several different marketing Sources (e.g. "leganto_postcard1", "leganto_poster1", "leganto_handout1") where you are using different QR codes to track usage of each. 
Adding unique values for each will allow you to track the Campaign over all, push how many clicks each individual Source had.
The Medium is for tracking and filtering the general medium of all Sources, so that we can compare different marketing usage such as emails vs print handouts.

To view the stats, you will need access to our Analytics account.
You can view the parameters or use them to filter, in the Acquisition > Traffic acquisition report.

*Note GA4 update:* Analytics upgraded to a new platform called GA4 in Aug 2023 (the older version UA has stopped collecting data). 
The use of utm parameters remains the same, however, how the options are reported is a bit different. 
In the defunct UA version, Campaign ID (utm_id) was required--in GA4 utm_id is not generally used, but utm_source, utm_medium, and utm_campaign should always be used. 

## Why qr-generator?

There are many "free" online platforms for creating QR codes, but some are spammy or risk user privacy.
If a service offers usage statistics or editable URLs, it is not providing clean QR codes, but instead is inserting a tracking short link that your user's traffic is directed through. 
Generally, this is an unnecessary trade off of your user's privacy and data for the slight convenience.
It can also be dangerous if the service goes out of business or is taken over by malicious interests--those links can be redirected anywhere out of your control.

This page provides an open source, non-commercial, client-side, self-hosted alternative (powered by the [QR Code Styling](https://github.com/kozakdenys/qr-code-styling) library).
