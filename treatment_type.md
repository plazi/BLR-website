
## Fields

### Current Zenodeo API treatments parameters

| field name | type | facet | Description |
| --- | --- | --- | --- |
| treatmentId | string | no | The unique ID of the treatment |
| format | string | no | Response format |
| page | integer | no | Starting page, defaults to 1 |
| size | integer | no | Number of records to fetch per query, defaults to 30 |
| treatmentTitle | string | no | Title of the article that contains this treatment |
| journalTitle | string | yes | Title of the journal |
| journalYear | string | yes | Year of the journal |
| authorityName | string | yes? | The name of the author(s) of the taxon (not necessarily the same as the authors of the journal article, but ommited if same as article authors) |
| authorityYear | string | no? | The year when the taxon name has been published |
| kingdom | string | yes | Higher category of the taxonomicName |
| phylum | string | yes | Higher category of the taxonomicName |
| order | string | yes | Higher category of the taxonomicName |
| family | string | yes | Higher category of the taxonomicName |
| genus | string | yes | Higher category of the taxonomicName |
| species | string | yes | The specific epithet of a Latin Binomen |
| rank | string | yes | The taxonomic rank of the taxon, e.g. species, family.
| q |string | no | Full text of the treatment |
| lat | number | no | Geographic coordinates where the specimen has been collected |
| lon | number | no | Geographic coordinates where the specimen has been collected |
