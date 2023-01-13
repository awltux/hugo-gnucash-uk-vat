# hugo-gnucash-uk-vat
Provides a minimalistic [website for gnucash-uk-vat instance used by Awltux Ltd](http://gnucash-uk-vat.awltux.trade/) using the Hugo static site generator.

These pages are primarily to meet the HMRC MTD requirements when requesting a public access token.

## Add Pages
Add a new page to /content/

```hugo add new-page-name.md```

## Build Website
Create the latest version of the websiet in public/

```hugo```

## Upload Website to AWS S3
Copy the contents of public/ to the S3 bucket in AWS.
