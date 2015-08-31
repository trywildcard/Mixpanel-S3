Mixpanel-S3
===============

Mixpanel-S3 is a simple Python library for exporting Mixpanel data to S3. It works by pulling data via [Mixpanel's export api](https://mixpanel.com/docs/api-documentation/data-export-api).

##Usage

Run ```./mixpanelS3 -h``` for usage instructions. Requires that [boto] is installed and configured properly.

    usage example: ./mixpanelS3 --apikey [mixpanel_key] --apisecret [mixpanel_secret] --startdate 2015-08-21 --enddate 2015-08-21 --bucket wildcard-datascience --destdir mixpanel/mixpanel-appstore

    Retrieve data from Mixpanel. Will use the MIXPANEL_KEY, MIXPANEL_SECRET and
    S3_BUCKET environment variables if they are set.

    optional arguments:
      -h, --help            show this help message and exit
      --bucket BUCKET       s3 bucket
      --apikey APIKEY       mixpanel api key
      --apisecret APISECRET
                            mixpanel api secret
      --startdate STARTDATE
                            start date
      --enddate ENDDATE     end date
      --tmpdir TMPDIR       Temporary directory
      --dry                 dry-run mode


You can find your Mixpanel keys by logging into your Mixpanel account, clicking the "Account" link on the upper right corner, and then selecting the "Projects" tab.
