## Idea
The idea is to provide a more powerful taxon-search that includes synonimic list and verification of valid names into the BLR website. This is based on [Reto's Synospecies](https://synospecies.factsmission.com/) service, which already returns synonimic lists. 

## Specs
A bar, either above the list or of results on the right side (we've to see mockups with the two implementations in order to decide), showing the mapped list of synonimies, turning each taxon name into a link to a new Zenodeo query. At the bottom an additional link to a query that will be composed by all included names should be added. This link is a particular important feature for the end user

## Actors' Responsibility

### Pensoft
- Will make the Synospecies API call, display the results as links, as described above

### Zenodeo
- Will provide a way to query taxon names (treatment titles) with more than one taxon, perhaps separated by a pre-defined separator (e.g. ";")
