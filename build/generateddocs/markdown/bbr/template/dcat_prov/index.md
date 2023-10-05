
# My Building Block (Schema)

`ogc.bbr.template.dcat_prov` *v0.1*

This Building Block serves as a template to create new ones

[*Status*](http://www.opengis.net/def/status): Under development

## Description

## Qui hastarum tectus Cithaeron iuvabat

Lorem markdownum vestigia sanguine rursus undis, suspenderat meo mox conlegerat
temperat sucos. Est graves dant sentire sanguinis flores respondent testari.

> Videri vias quid Ausoniae sua flores ante, reminiscitur fuit est. Semel
> [hectora](http://silvaque.org/) peregrinaeque rudem exercent in, Troiana si
> Asida instabilesque somno sed.

## Iam vota cui dilataque peterem

Tinxit lumina lacer liquidarum Aiax si mergitur sed fueris capitisque **et
cadit** contigerant rectum [ferar](http://prosternit.com/quoque.html) temperat.
Monet caput adsensere Ityn furentibus gelidos.
## Examples

### This is an example with just a description and no code snippets.
This is the content of the example.

In **Markdown** format.
#### ttl
```ttl
# baseURI: https://dcat.example.org/basic-example

@prefix adms: <https://www.w3.org/ns/adms#> .
@prefix dcat: <http://www.w3.org/ns/dcat#> .
@prefix dct: <http://purl.org/dc/terms/> .
@prefix ex: <https://dcat.example.org/> .
@prefix foaf: <http://xmlns.com/foaf/0.1/> .
@prefix geosparql: <http://www.opengis.net/ont/geosparql#> .
@prefix locn: <http://www.w3.org/ns/locn#> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix time: <http://www.w3.org/2006/time#> .
@prefix w3cgeo: <http://www.w3.org/2003/01/geo/wgs84_pos#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

ex:basic-example
  a owl:Ontology ;
.
ex:catalog
  a dcat:Catalog ;
  dct:language <http://id.loc.gov/vocabulary/iso639-1/en> ;
  dct:publisher ex:transparency-office ;
  dct:title "Imaginary Catalog"@en ;
  rdfs:label "Imaginary Catalog"@en ;
  dcat:dataset ex:dataset-001 ;
  dcat:dataset ex:dataset-002 ;
  dcat:dataset ex:dataset-003 ;
  foaf:homepage <http://example.org/catalog> ;
.
ex:dataset-001
  a dcat:Dataset ;
  dct:accrualPeriodicity <http://purl.org/linked-data/sdmx/2009/code#freq-W> ;
  dct:creator ex:finance-employee-001 ;
  dct:issued "2011-12-05"^^xsd:date ;
  dct:language <http://id.loc.gov/vocabulary/iso639-1/en> ;
  dct:modified "2011-12-15"^^xsd:date ;
  dct:publisher ex:finance-ministry ;
  dct:spatial <http://sws.geonames.org/6695072/> ;
  dct:temporal <http://reference.data.gov.uk/id/quarter/2006-Q1> ;
  dct:title "Imaginary dataset"@en ;
  dcat:contactPoint <http://example.org/transparency-office/contact> ;
  dcat:distribution ex:dataset-001-csv ;
  dcat:keyword "accountability"@en ;
  dcat:keyword "payments"@en ;
  dcat:keyword "transparency"@en ;
  dcat:spatialResolutionInMeters 30.0 ;
  dcat:temporalResolution "P1D"^^xsd:duration ;
.
ex:dataset-001-csv
  a dcat:Distribution ;
  dct:title "CSV distribution of imaginary dataset 001"@en ;
  dcat:byteSize "5120"^^xsd:decimal ;
  dcat:downloadURL <http://www.example.org/files/001.csv> ;
  dcat:mediaType <https://www.iana.org/assignments/media-types/text/csv> ;
.
ex:transparency-office
  a foaf:Organization ;
  rdfs:label "Transparency Office"@en ;
.

```

## Sources

* [Sample source document](https://example.com/sources/1)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/dcat-ddi-cdif](https://github.com/ogcincubator/dcat-ddi-cdif)
* Path: `_sources/dcat_prov`

