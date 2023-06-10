# CHEK profiles

## CityJSON uplift definition

The `cityjson/` subdirectory hosts several CityJSON sample files and drafts for
[JSON Uplift Definitions](https://opengeospatial.github.io/ogc-na-tools/tutorials/#how-to-create-a-json-ld-uplift-context-definition)
that can be used to convert CityJSON into RDF.

The configuration for the uplift process is defined in `.ogc/catalog.ttl`.

A GitHub workflow updates the RDF versions of the JSON files on every push.