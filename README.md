# DCAT feeds for MELODIES's CKAN Demo

A collection of GeoDCAT-AP catalogs written in JSON-LD which are suitable as feeds for CKAN.

The [MELODIES CKAN demo](http://ckan-demo.melodiesproject.eu/) is set up to harvest the files `WP[2-10].jsonld` in this repository every day (or manually on request, please contact Maik Riechert for that). On each harvest, existing datasets are updated, new ones are added, and old ones which don't exist anymore are removed.

**IMPORTANT**: When you create new dataset entries, ALWAYS use a new unique URL as `"@id"` which doesn't appear in any other feed, for example `http://melodiesproject.eu/datasets/wp6/temperature/2012/12`. If a URL appears twice amongst any of the feeds CKAN will **crash** on harvesting due to [a bug](https://github.com/ckan/ckanext-harvest/issues/162).
