# Edmonlytica - Server Side Tag

Edmonlytica is a proof of concept for making your own digital analytics stream using GTM Server Side and BigQuery.  See the blog post for details:
https://code.markedmondson.me/edmondlytica/

## Dependencies

This is the server side tag to be imported into GTM Browser Side.  It works in conjunction with the [Edmonlytica GTM Server Side Client](https://github.com/MarkEdmondson1234/edmonlytica-server-side-client) and the [Edmonlytica GTM Browser Tag](https://github.com/MarkEdmondson1234/edmonlytica-browser-template), which need to be installed as well to work.

## Functionality

This takes the event data passed to it from the GTM Server Side Client, and does the BigQuery API call to write that event data to BigQuery.

You will need to configure the BigQuery table to have the following schema:


* event: STRING
* referrer: STRING
* ts: STRING
* eventId: STRING
* custom: STRING
* sessionId: STRING
* event_name: STRING
* page: STRING
