# CHEK profiles

This repository defines profiles of standards used in the [CHEK project](https://chekdbp.eu/).

It uses automated scripts to transform and validate implementation patterns into a semantic model that can be matched to the business rules.  This transformation allows multiple forms of data to coexist (as required to integrate different systems) whilst simplifying using a single profile specification that meets this goal. 

The high level architecture (and implementation status) is described in this workflow:

![](https://lucid.app/publicSegments/view/d8b1a916-9687-4cb4-9a9c-fd65a8b018a3/image.png)

A canonical OWL representation of CityGML is the key blocker. 

The "Topo-features" model for handling topological relationships in a manner compatible with OGC-API-Features has been prototyped in a related project and will be migrated to an OGC repository to support ongoing development, testing and reuse.

## CityJSON uplift definition

The `cityjson/` subdirectory hosts several CityJSON sample files and drafts for
[JSON Uplift Definitions](https://opengeospatial.github.io/ogc-na-tools/tutorials/#how-to-create-a-json-ld-uplift-context-definition)
that can be used to convert CityJSON into RDF.

The configuration for the uplift process is defined in `.ogc/catalog.ttl`.

A GitHub workflow updates the RDF versions of the JSON files on every push.
