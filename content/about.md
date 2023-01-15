---
title: "About"
date: 2023-01-12T15:45:52Z
---

# gnucash-uk-vat.awltux.trade
This is a git fork of the [gnucash-uk-vat](https://github.com/cybermaggedon/gnucash-uk-vat) repository.
The source code can be cloned from the [forked repository](https://github.com/awltux/gnucash-uk-vat)

The gnucash-uk-vat bridge uses a configuration file to declare which GnuCash SQLite file to use 
and a list of GnuCash accounts that correlate to the HMRC VAT submission fields.
When invoked, the gnucash-uk-vat bridge:
* starts a local REST API to accept the OAuth redirect.
* prints a URL to the console that the user must use to authenticate with the HMRC OAuth service. The URL contains a redirectURL parameter for the local REST API. 
Open the URL in a browser and log into the HMRC OAuth service. A successful authentication will redirects the client browser to the local REST API, appending the OAuth token to the URL.
The application can then use the OAuth token when calling the MTD VAT REST API.
