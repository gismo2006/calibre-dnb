# DNB metadata plugin for Calibre

A Calibre metadata source plugin that uses the catalogue (https://portal.dnb.de) of the Deutsche Nationalbibliothek (DNB) to retrieve metadata.
It supports retrieval of DNB-IDN, ISBN, authors, title, edition, tags, pulication date, languages, publisher, comments, series, series index and cover.

For books without series information it can try to extract series and series index from the title.
GND and/or non-GND subjects can be used as tags.

### Requirements:

None.

For better performance and stability it is recommended to use a personal SRU Access Token. The Token is free of charge, you can get it from the DNB.
With this token this plugin will use DNB's SRU API, without token it will do web scraping. The downloaded metadata is the same in each case.

### Installation:

1. Download the latest release (https://github.com/citronalco/calibre-dnb/releases/download/v2.0.5/dnb-metadata-plugin-2.0.5.zip)
1. Start Calibre
1. In "Preferences", section "Advanced" click on "Plugins"
1. "Load plugin from file"
1. Choose the downloaded dnb-metadata-plugin-2.0.5.zip
1. Restart Calibre

### How to get a SRU Access Token:

1. Create a free account at https://portal.dnb.de/myAccount/register.htm
1. Write an email to schnittstellen-service@dnb.de and ask them to enable SRU Access Token generation for your account.
1. Log in into your DNB account and create an Access Token.
1. Enter the Access Token into this plugin's settings page.

The Token is free of charge.

### Limitations and caveats

- The returned publication date contains only the year, not the precise date.
