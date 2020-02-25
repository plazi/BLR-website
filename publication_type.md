# Publication Object Type

- [Fields](#fields)
  - [Zenodeo API image parameters](#zenodeo-api-treatments-parameters)
  - [Zenodeo response fields](#zenodeo-response-fields)
- [Displays](#displays)
  - [Search result display](#search-result-display)
  - [Image page display](#image-page-display)
- [Sample Zenodeo API response (image)](#sample-zenodeo-api-response)

## Fields

### Zenodeo API publication parameters

| field name | type | facet | Description |
| --- | --- | --- | --- |

Currently, Zenodeo doesn't support publications.

### Zenodeo response fields
| field | facet | sort |result display | notes |
| --- | --- | --- | --- | --- |

## Displays

### Search result display

* publication title
* publication authors
* publication info = volume, issue, pages
* if it has treatments (numbers)
* if it has images (numbers)
* DOI
* zenodo dep_id (only if the DOI is not from zenodo?)


### Publication page display


## Sample Zenodeo API response

```
```

## Sample Zenodo API response

```
{
  "files": [
    {
      "links": {
        "self": "https://zenodo.org/api/files/c9b9d61a-c05d-43a4-bdd3-118c25f3247e/CheckList_article_19752.pdf"
      }, 
      "checksum": "md5:2d297be299ded66a62160718ef72a4de", 
      "bucket": "c9b9d61a-c05d-43a4-bdd3-118c25f3247e", 
      "key": "CheckList_article_19752.pdf", 
      "type": "pdf", 
      "size": 1524478
    }
  ], 
  "owners": [
    1161
  ], 
  "doi": "10.15560/13.3.2151", 
  "stats": {}, 
  "links": {
    "doi": "https://doi.org/10.15560/13.3.2151", 
    "latest_html": "https://zenodo.org/record/1143410", 
    "bucket": "https://zenodo.org/api/files/c9b9d61a-c05d-43a4-bdd3-118c25f3247e", 
    "badge": "https://zenodo.org/badge/doi/10.15560/13.3.2151.svg", 
    "html": "https://zenodo.org/record/1143410", 
    "latest": "https://zenodo.org/api/records/1143410"
  }, 
  "created": "2018-01-09T16:49:48.664135+00:00", 
  "updated": "2018-01-09T17:40:13.724660+00:00", 
  "conceptrecid": "1143409", 
  "revision": 2, 
  "id": 1143410, 
  "metadata": {
    "access_right_category": "success", 
    "doi": "10.15560/13.3.2151", 
    "description": "The geographic ranges in Brazil of 4 species of Neriidae are widened. New records are recorded of the following species and Brazilian states: <em>Eoneria blanchardi</em> Acz\u00e9l, 1951 from Pernambuco and Para\u00edba, Glyphidops carrerai Acz\u00e9l, 1961 and <em>Glyphidops filosus</em> (Fabricius, 1805) from Bahia and Para\u00edba, and <em>Nerius pilifer</em> Fabricius, 1805 from Para\u00edba. A referential map is included to these species.", 
    "license": {
      "id": "CC-BY-4.0"
    }, 
    "title": "New distribution records for Neriidae (Diptera, Schizophora) from northeastern Brazil", 
    "journal": {
      "volume": "13", 
      "issue": "(3)", 
      "pages": "1-5", 
      "title": "Check List"
    }, 
    "relations": {
      "version": [
        {
          "count": 1, 
          "index": 0, 
          "parent": {
            "pid_type": "recid", 
            "pid_value": "1143409"
          }, 
          "is_last": true, 
          "last_child": {
            "pid_type": "recid", 
            "pid_value": "1143410"
          }
        }
      ]
    }, 
    "imprint": {
      "publisher": "Pensoft Publishers"
    }, 
    "communities": [
      {
        "id": "biosyslit"
      }
    ], 
    "keywords": [
      "Atlantic Forest species", 
      "Bahia", 
      "Caatinga species", 
      "cactus flies", 
      "Nerioidea", 
      "Para\u00edba", 
      "Pernambuco"
    ], 
    "publication_date": "2017-06-22", 
    "creators": [
      {
        "name": "Braga, Izabela"
      }, 
      {
        "affiliation": "Universidade Federal da Para\u00edba, BRAZIL, Brazil", 
        "name": "Pereira-Colavite, Alessandre"
      }, 
      {
        "name": "Cre\u00e3o-Duarte, Antonio"
      }
    ], 
    "access_right": "open", 
    "resource_type": {
      "subtype": "article", 
      "type": "publication", 
      "title": "Journal article"
    }
  }
}
```
