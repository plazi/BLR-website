# Biodiversity Literature Repository Website

## Vision


## Static links
1. About - about BLR
2. Liberating Data - political information about the process
3. How BLR Works - inner workings about the process and the involved agents
4. Contribute - how to contribute
5. Blog - external platform linked to the website

## Search System
The user will choose between the different data available for search, and then, choose which information should be queried. 

Advanced search functionality would be available through filters.

### Query types
1. Taxon [Current Limitation 1]
    Return distinct of all treatments which has the search term in either:
          treatmentTitle, kingdom, phylum, order, family, genus, species
2. Journal
    Return distinct of all treatments which has the search term in:
         journalTitle
3. Author
    Return distinct of all treatments which has the search term in:
         authorityName
4. Institution/Collection** (search grbio for institution -> get the code and seach q matchword)
5. Community (to do)

### Filter options

### Data types
1. Taxonomic treatments (searched on Zenodeo)
2. Images (searched on Zenodo)
3. Publications (searched on ?)

#### Taxonomic Treatments
1. Taxon Rank
2. Taxonomic Status
3. Author*
4. Journal*
5. Instituton/Collection (Current Limitation #2)
6. Communities
7. Dates

'* If the query type is author or journal, this filter option wouldn't be available. 

#### Images (see Current Limitation #3)

#### Publication (see To be decided #1)

## Index Page
* Header(BLR logo, links)
* Dynamic map, just like the one in Plazi's website
* Search box
* Footer ('powered by', social media links)

## Search Page

1. Header (BLR logo, links)
2. Filter
2.1 Dashboards
2.2 Results*
5. Footer ('Powered by', social media links)

'* Each **data type** would be presented in the result list with:

### Taxonomic Treatments

1. Labels (Figures, Geographic Coordinates, Taxonomic Keys - if present)
1. Title or Concept Label
2. Reference
3. Links to GBIF/Zenodo/TB

### Images
1. Labels (Treatments - if available)
1. Title or Concept Label
2. Reference
3. Links to GBIF/Zenodo/TB

### Publications

1. Labels (Treatments, Figures - if present)
1. Title or Concept Label
2. Reference
3. Links to GBIF/Zenodo/TB

## Unit Pages

### Taxonomic Treatments
1. Header (BLR logo, links)
2. Reference
3. Treatment

3.1. Links to Alternative Sources (Zenodo, GBIF, TB)

3.2. Dashboards - Taxonomic ranking tree with available treatments per rank

3.3. "Has parts" (figures, keys, treatment citations)

4. Figures included
5. Map, if coordinates are available
6. Footer ('Powered by', social media links)

### Image
1. Header (BLR logo, links)
2. Reference
3. Image

3.1. Links to Alternative Sources

4. Caption
4. Related Items*
5. Footer ('Powered by', social media links)

### Publications
1. Header (BLR logo, links)
2. Reference
3. Render of PDF

3.1. Links to Alternative Sources

4. Related Items*
5. Footer ('Powered by', social media links)

'* A new query would have to be made based on an specific, pre-defined information of the clicked image, to retrieve and show some related items in all three 'unit searches'.


## Current limitations

1. Taxonomic treatments have fixed information about taxonomic ranks, meaning that, if the classification changes, treatments won't have this part of their metadata updated. In sum: if a species of a given treatement is transferred to a different genus, the genus included in the treatment metadata will be outdate. This means that querrying the data won't bring results that reflect the most updated classification hypothesis available for that given taxon.

2. More than one collection can belong to the same institution. Thus, it would be nice to be able to query the institution's full name to access all treatments, or images or publications, associated with that. The problem here is the correspondance in between collection codes and institutions full names, which is available on GBIF but not integrated in Zenodeo/Zenodo.

3. Images are queried in Zenodo, which doesn't returns enough metadata to have all desired filters applied (for instance, there is no information about taxonomic ranks in the image metadata, for many reasons).

## To be Decided

1. When working with publications, should we query Zenodeo or Zenodo? Publication metadata also will have taxononomic ranking missing, if I'm remember this correctly.

2. Geographical queries.

## Requested features

1. Zenodeo - OpenBioDiv, so we can have a list of treatment IDs to be queried based on current, most acceptable hypotheses of taxonomic classification. 
2. Zenodeo - GBIF, so we can translate institutuons' full names into collection codes, and then, query Zenodeo.

### Related projects:

* https://zenodeo.punkish.org/ / https://github.com/punkish/zenodeo
