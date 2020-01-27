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
| *doi* | |  |  |
| *citedByTreatment* | | | |
| *publicationTitle* | | | needs to be added to zenodo metadata |
| *kingdom* | | | needs to be added as custom metadata |
| *phylum* | | |  needs to be added as custom metadata |
| *order* | | |  needs to be added as custom metadata |
| *family* | | |  needs to be added as custom metadata |
| *genus* | | |  needs to be added as custom metadata |
| *species* | | |  needs to be added as custom metadata |

According to https://zenodeo.punkish.org/docs#/v2/getV2Images (2019-09-12, 17:33), there are  o parameters for images.

### Zenodeo response fields
| field | facet | sort |result display | notes |
| --- | --- | --- | --- | --- |
| title | no | no | yes | |
| creators | yes | no | yes | | 
| images | no | no | yes | |
| thumb250 |  no | no | yes | |

## Displays

### Search result display

* image thumbnail
* image caption = title
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

## Sample Zenodo API response (for the same record as above)

```
{
  "conceptdoi": "10.5281/zenodo.3406430",
  "conceptrecid": "3406430",
  "created": "2019-09-12T14:01:35.346608+00:00",
  "doi": "10.5281/zenodo.3406431",
  "files": [
    {
      "bucket": "539746bd-3ab0-4b62-8b63-b2921a421fd6",
      "checksum": "md5:f0d8851fdb786cb6d286bb92b56a8648",
      "key": "figure.png",
      "links": {
        "self": "https://zenodo.org/api/files/539746bd-3ab0-4b62-8b63-b2921a421fd6/figure.png"
      },
      "size": 6502106,
      "type": "png"
    }
  ],
  "id": 3406431,
  "links": {
    "badge": "https://zenodo.org/badge/doi/10.5281/zenodo.3406431.svg",
    "bucket": "https://zenodo.org/api/files/539746bd-3ab0-4b62-8b63-b2921a421fd6",
    "conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.3406430.svg",
    "conceptdoi": "https://doi.org/10.5281/zenodo.3406430",
    "doi": "https://doi.org/10.5281/zenodo.3406431",
    "html": "https://zenodo.org/record/3406431",
    "latest": "https://zenodo.org/api/records/3406431",
    "latest_html": "https://zenodo.org/record/3406431",
    "self": "https://zenodo.org/api/records/3406431",
    "thumb250": "https://zenodo.org/api/iiif/v2/539746bd-3ab0-4b62-8b63-b2921a421fd6:d292f847-9eef-4066-9407-3d1a439a0506:figure.png/full/250,/0/default.png",
    "thumbs": {
      "10": "https://zenodo.org/record/3406431/thumb10",
      "50": "https://zenodo.org/record/3406431/thumb50",
      "100": "https://zenodo.org/record/3406431/thumb100",
      "250": "https://zenodo.org/record/3406431/thumb250",
      "750": "https://zenodo.org/record/3406431/thumb750",
      "1200": "https://zenodo.org/record/3406431/thumb1200"
    }
  },
  "metadata": {
    "access_right": "open",
    "access_right_category": "success",
    "communities": [
      {
        "id": "biosyslit"
      }
    ],
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
    "description": "FIGURE 29. Antichiropus procerus Car, n. sp., holotype male (WAM T144538):A–B habitus: A, lateral view; B, dorsal view; C–F, left gonopod: C, posterior view; D, anterior view; E, medial view; F, lateral view; Abbreviations: C, coxa; F, femorite; MFP, main femoral process; PF, prefemur; prof, prolongation of femorite; S, solenomere; sp1 and sp2, solenomere processes 1 and 2. Scale bars: A = 2 mm; B = 1 mm; C–F = 0.5 mm.",
    "doi": "10.5281/zenodo.3406431",
    "journal": {
      "issue": "1",
      "pages": "1-71",
      "title": "Zootaxa",
      "volume": "4617"
    },
    "keywords": [
      "Biodiversity",
      "Taxonomy",
      "Animalia",
      "Arthropoda",
      "Diplopoda",
      "Polydesmida",
      "Paradoxosomatidae",
      "Antichiropus"
    ],
    "license": {
      "id": "notspecified"
    },
    "publication_date": "2019-06-17",
    "related_identifiers": [
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD24FFD4C8BBB5E3FD85FE63",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD3CFFCEC8BBB438FD83FE63",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD34FFC5C8BBB485FBEDFD88",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD69FF99C8BBB7C9FAD5F956",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "10.11646/zootaxa.4617.1.1",
        "relation": "isPartOf",
        "scheme": "doi"
      },
      {
        "identifier": "urn:lsid:plazi.org:pub:FFD9FFADAD28FFDBC82CB750FFABFFB7",
        "relation": "isPartOf",
        "scheme": "lsid"
      },
      {
        "identifier": "http://publication.plazi.org/id/FFD9FFADAD28FFDBC82CB750FFABFFB7",
        "relation": "isPartOf",
        "scheme": "url"
      },
      {
        "identifier": "https://zenodo.org/record/3248154",
        "relation": "isPartOf",
        "scheme": "url"
      },
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD3CFFCEC8BBB438FD80FE63",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "http://treatment.plazi.org/id/03E087D5AD34FFC5C8BBB485FBE0FD88",
        "relation": "isCitedBy",
        "scheme": "url"
      },
      {
        "identifier": "10.11646/zootaxa.4617.1.1",
        "relation": "isPartOf",
        "scheme": "doi"
      },
      {
        "identifier": "10.5281/zenodo.3406430",
        "relation": "isVersionOf",
        "scheme": "doi"
      }
    ],
    "relations": {
      "version": [
        {
          "count": 1,
          "index": 0,
          "is_last": true,
          "last_child": {
            "pid_type": "recid",
            "pid_value": "3406431"
          },
          "parent": {
            "pid_type": "recid",
            "pid_value": "3406430"
          }
        }
      ]
    },
    "resource_type": {
      "subtype": "figure",
      "title": "Figure",
      "type": "image"
    },
    "title": "FIGURE 29. Antichiropus procerus Car, n in The millipede genus Antichiropus (Diplopoda: Polydesmida: Paradoxosomatidae), part 3: species of the Pilbara bioregion of Western Australia"
  },
  "owners": [
    1161
  ],
  "revision": 3,
  "stats": {
    "downloads": 9,
    "unique_downloads": 7,
    "unique_views": 13,
    "version_downloads": 9,
    "version_unique_downloads": 7,
    "version_unique_views": 13,
    "version_views": 13,
    "version_volume": 58518954,
    "views": 13,
    "volume": 58518954
  },
  "updated": "2019-09-13T10:31:43.870563+00:00"
}
```
