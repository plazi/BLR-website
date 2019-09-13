# Image Object Type

- [Fields](#fields)
  - [Zenodeo API image parameters](#zenodeo-api-treatments-parameters)
  - [Zenodeo response fields](#zenodeo-response-fields)
- [Displays](#displays)
  - [Search result display](#search-result-display)
  - [Image page display](#image-page-display)
- [Sample Zenodeo API response (image)](#sample-zenodeo-api-response)

## Fields

### Zenodeo API images parameters

| field name | type | facet | Description |
| --- | --- | --- | --- |

According to https://zenodeo.punkish.org/docs#/v2/getV2Images (2019-09-12, 17:33), there are  o parameters for images.

### Zenodeo response fields
| field | facet | sort |result display | notes |
| --- | --- | --- | --- | --- |
| title | no | no | yes | |
| creators | yes | no | yes | | 
| images | no | yes | yes | |
| thumb250 |  no | no | yes | |

## Displays

### Search result display

* image thumbnail
* image caption
* publication info = articleTitle + journalTitle + journalVolume + journalIssue + journalYear + articleDoi + articlePages + pages
* link to zenodo record = doi
* treatment flag, if belongs to a treatment


### Image page display


## Sample Zenodeo API response

```
"https://zenodo.org/api/records/3406431": {
        "title": "FIGURE 29. Antichiropus procerus Car, n in The millipede genus Antichiropus (Diplopoda: Polydesmida: Paradoxosomatidae), part 3: species of the Pilbara bioregion of Western Australia",
        "creators": [
          {
            "name": "Car, Catherine A."
          },
          {
            "name": "Harvey, Mark S."
          },
          {
            "name": "Hillyer, Mia J."
          },
          {
            "name": "Huey, Joel A."
          }
        ],
        "images": [
          "https://zenodo.org/api/files/539746bd-3ab0-4b62-8b63-b2921a421fd6/figure.png"
        ],
        "thumb250": "https://zenodo.org/api/iiif/v2/539746bd-3ab0-4b62-8b63-b2921a421fd6:d292f847-9eef-4066-9407-3d1a439a0506:figure.png/full/250,/0/default.png"
      },
```

## Sample Zenodo API response

```
{
  "files": [
    {
      "links": {
        "self": "https://zenodo.org/api/files/1982e601-5afd-4d3f-9061-57f385275e6c/figure.png"
      }, 
      "checksum": "md5:6a7cb5304795726d1b5a153c05b0d8b0", 
      "bucket": "1982e601-5afd-4d3f-9061-57f385275e6c", 
      "key": "figure.png", 
      "type": "png", 
      "size": 1138196
    }
  ], 
  "owners": [
    1161
  ], 
  "doi": "10.5281/zenodo.995792", 
  "stats": {}, 
  "links": {
    "doi": "https://doi.org/10.5281/zenodo.995792", 
    "conceptdoi": "https://doi.org/10.5281/zenodo.995791", 
    "thumb250": "https://zenodo.org/api/iiif/v2/1982e601-5afd-4d3f-9061-57f385275e6c:f59075a0-cb4c-40f1-aa85-b8c796094006:figure.png/full/250,/0/default.png", 
    "bucket": "https://zenodo.org/api/files/1982e601-5afd-4d3f-9061-57f385275e6c", 
    "conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.995791.svg", 
    "html": "https://zenodo.org/record/995792", 
    "latest_html": "https://zenodo.org/record/995792", 
    "badge": "https://zenodo.org/badge/doi/10.5281/zenodo.995792.svg", 
    "latest": "https://zenodo.org/api/records/995792"
  }, 
  "conceptdoi": "10.5281/zenodo.995791", 
  "created": "2017-09-25T06:26:30.283973+00:00", 
  "updated": "2017-09-25T06:26:30.505485+00:00", 
  "conceptrecid": "995791", 
  "revision": 1, 
  "id": 995792, 
  "metadata": {
    "access_right_category": "success", 
    "doi": "10.5281/zenodo.995792", 
    "description": "FIGURES 47 \u2013 49. Bomis hippoponoi, male. 47 habitus, dorsal; 48 \u2013 49 left pedipalp (48 ventral, 49 retrolateral). Scale bars: (47) = 1 mm; (48, 49) = 0.1 mm.", 
    "license": {
      "id": "notspecified"
    }, 
    "title": "FIGURES 47 \u2013 49. Bomis hippoponoi, male. 47 in Redescription of Bomis larvata L. Koch, 1874 with the description of a new Australian species", 
    "relations": {
      "version": [
        {
          "count": 1, 
          "index": 0, 
          "parent": {
            "pid_type": "recid", 
            "pid_value": "995791"
          }, 
          "is_last": true, 
          "last_child": {
            "pid_type": "recid", 
            "pid_value": "995792"
          }
        }
      ]
    }, 
    "keywords": [
      "Biodiversity", 
      "Taxonomy", 
      "Animalia", 
      "Arthropoda", 
      "Arachnida", 
      "Araneae", 
      "Thomisidae", 
      "Bomis"
    ], 
    "publication_date": "2017-09-25", 
    "creators": [
      {
        "name": "Kr\u00f3likowska, Sylwia"
      }
    ], 
    "access_right": "open", 
    "resource_type": {
      "subtype": "figure", 
      "type": "image", 
      "title": "Figure"
    }, 
    "related_identifiers": [
      {
        "scheme": "url", 
        "relation": "isCitedBy", 
        "identifier": "http://treatment.plazi.org/id/03EF1F6BFFD3FF80FF16F8ECFEEF0187"
      }, 
      {
        "scheme": "doi", 
        "relation": "isPartOf", 
        "identifier": "10.11646/zootaxa.4323.4.1"
      }, 
      {
        "scheme": "lsid", 
        "relation": "isPartOf", 
        "identifier": "urn:lsid:plazi.org:pub:FFD66713FFDBFF8FFF81FFFDFFBB002B"
      }, 
      {
        "scheme": "url", 
        "relation": "isPartOf", 
        "identifier": "https://zenodo.org/record/995772"
      }, 
      {
        "scheme": "doi", 
        "relation": "isVersionOf", 
        "identifier": "10.5281/zenodo.995791"
      }
    ]
  }
}
```
