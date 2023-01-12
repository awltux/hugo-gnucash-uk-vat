---
title: "About"
date: 2023-01-12T15:45:52Z
---

# gnucash-uk-vat.awltux.trade
This is a git fork of the [gnucash-uk-vat]{https://github.com/cybermaggedon/gnucash-uk-vat} repository.
The source code can be cloned from the [forked repository]{https://github.com/awltux/gnucash-uk-vat}

The gnucash-uk-vat bridge uses a configuration file to declare which GnuCash SQLite file to use 
and a list of GnuCash accounts that reference the HMRC VAT submission field values.
The bridge contacts the HMRC OAuth service, providing the redirect URL of a local REST API. 
The HMRC OAuth service redirects to this REST API, appending the OAuth token to the URL so 
that the application can use the OAuth token when calling the MTD REST API.
