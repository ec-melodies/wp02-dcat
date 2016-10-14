# DCAT feeds of MELODIES datasets

A GeoDCAT-AP catalogue written in JSON-LD and loaded in the [MELODIES Demo Portal](http://ec-melodies.github.io/demo-portal).

**IMPORTANT**: When you create new dataset entries, ALWAYS use a new unique URL as `"@id"` which doesn't appear in any other feed, for example `http://melodiesproject.eu/datasets/wp6/temperature/2012/12`. If a URL appears twice amongst any of the feeds CKAN will **crash** on harvesting due to [a bug](https://github.com/ckan/ckanext-harvest/issues/162).

## FAQ

### `observedProperty` URLs

If you have a CF standard name, then use http://vocab.nerc.ac.uk/standard_name/sea_water_temperature/ where the last URL part contains the standard name.

For any other code list names, try to find it in one of the many collections at http://vocab.nerc.ac.uk/collection/.
