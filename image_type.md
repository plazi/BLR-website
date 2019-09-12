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

* to be adde


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
