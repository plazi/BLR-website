# Treatment Object Type

- [Fields](#fields)
  - [Zenodeo API treatments parameters](#zenodeo-api-treatments-parameters)
  - [Zenodeo response fields](#zenodeo-response-fields)
- [Displays](#displays)
  - [Search result display](#search-result-display)
  - [Treatment page display](#treatment-page-display)
- [Sample Zenodeo API response (treatmentID)](#sample-zenodeo-api-response-treatmentid)

## Fields

### Zenodeo API treatments parameters

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
| *status*

### Zenodeo response fields
| field | facet | sort |result display | notes |
| --- | --- | --- | --- | --- |
| treatmentId | no | no | no | |
| treatmentTitle | no | no | yes | | 
| treatmentAuthors | no | yes | yes | |
| pages |  no | no | yes | |
| doi |  no | no | yes | |
| zenodoDep | no | no | no | |
| publicationDate |  no | no | no | |
| *articleTitle* |  no |  no | yes | needed |
| *articleDoi* | no | no | yes | needed |
| journalTitle | yes | no | yes | | 
| journalYear |  yes | yes | yes | | 
| journalVolume |  yes | no | yes | | 
| journalIssue | no | no | yes | |  
| authorityName |  no | no | yes? | | 
| authorityYear |  no | no | yes? | | 
| kingdom |  yes | no | no? | | 
| phylum | yes | no | no? | |  
| order | yes | no | no? | | 
| family | yes | no | no? | | 
| genus | yes | no | no? | |  
| species | yes | no? | no? | |  
| status | yes | no | yes | |  
| rank | yes | no | no | |
| materialsCitations | no? | yes (count) | no | can facet on contains materialsCitations |
| figureCitations | no? | yes (count) | no | can facet on "contains figureCitations"|
| treatmentCitations? | no? | yes (count) | no | can facet on "contains treatmentCitations"|

## Displays

### Search result display

* treatmentTitle
* treatmentAuthors
* publication info = *articleTitle* + journalTitle + journalVolume + journalIssue + journalYear + *articleDoi* + *articlePages* + pages
* status
* link to zenodo record = doi
* link to treatmentbank = "http://treatment.plazi.org/id/" + treatmentID
* image count = count(figureCitations items)
* materials count = count(materialsCitations items)


### Treatment page display


## Sample Zenodeo API response (treatmentID)

```
{
	"value": {
		"num-of-records": 40,
		"search-criteria": {
			"facets": "true",
			"page": "1",
			"q": "Maratus",
			"size": "30",
			"sortBy": "treatmentId:ASC",
			"stats": "true",
			"resource": "treatments",
			"limit": 30,
			"offset": 0
		},
		"_links": {
			"self": {
				"href": "https://zenodeo.punkish.org/treatments?facets=true&page=1&q=Maratus&resource=treatments&size=30&sortBy=treatmentId:ASC&stats=true"
			}
		},
		"records": [
			{
				"id": 96939,
				"treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D",
				"treatmentTitle": "Maratus felinus Schubert, 2019, sp. nov.",
				"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
				"zenodoDep": "2588669",
				"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
				"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
				"publicationDate": "2019-03-05",
				"journalTitle": "Zootaxa",
				"journalYear": "2019",
				"journalVolume": "4564",
				"journalIssue": "1",
				"pages": "81–100",
				"authorityName": "Schubert",
				"authorityYear": "2019",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "felinus",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "Habitus images of living holotype  <b>Maratus</b> felinus   sp. nov.  (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.     FIGURE 18. Habitus images of preserved holotype  <b>Maratus</b> felinus   sp. nov.  (WAM–T147353): A, dorsal view; B, ventral view; C, anterior",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 96940,
				"treatmentId": "03FE87F49708FF92FF15F958FC94BB2E",
				"treatmentTitle": "Maratus aquilus Schubert, 2019, sp. nov.",
				"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
				"zenodoDep": "2588669",
				"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
				"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
				"publicationDate": "2019-03-05",
				"journalTitle": "Zootaxa",
				"journalYear": "2019",
				"journalVolume": "4564",
				"journalIssue": "1",
				"pages": "81–100",
				"authorityName": "Schubert",
				"authorityYear": "2019",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "aquilus",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "Living male paratype  <b>Maratus</b> aquilus   sp. nov.  ,  M. combustus   sp. nov.  , and  M. felinus   sp. nov.  performing courtship display to nearby female: A, Courtship display of male  <b>Maratus</b> aquilus   sp. nov.  ; B, courtship display of  <b>Maratus</b> combustus   sp. nov.  ; C, courtship display  of <b>Maratus</b> felinus  sp. nov.     Diagnosis. This species",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 96941,
				"treatmentId": "03FE87F49708FF94FF15F999FEA2BBAD",
				"treatmentTitle": "Maratus Karsch 1878",
				"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
				"zenodoDep": "2588669",
				"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
				"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
				"publicationDate": "2019-03-05",
				"journalTitle": "Zootaxa",
				"journalYear": "2019",
				"journalVolume": "4564",
				"journalIssue": "1",
				"pages": "81–100",
				"authorityName": "Karsch",
				"authorityYear": "1878",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "genus",
				"context": "Genus  <b>Maratus</b> Karsch, 1878          <b>Maratus</b>  Karsch, 1878 : 27   . Type species, by monotypy:  <b>Maratus</b> amabilis Karsch, 1878  , in   Bonnet, 1957: 2713.",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 96942,
				"treatmentId": "03FE87F4970EFF98FF15F9CBFDB7BE25",
				"treatmentTitle": "Maratus combustus Schubert, 2019, sp. nov.",
				"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
				"zenodoDep": "2588669",
				"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
				"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
				"publicationDate": "2019-03-05",
				"journalTitle": "Zootaxa",
				"journalYear": "2019",
				"journalVolume": "4564",
				"journalIssue": "1",
				"pages": "81–100",
				"authorityName": "Schubert",
				"authorityYear": "2019",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "combustus",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "Habitus images of living holotype  <b>Maratus</b> combustus   sp. nov.  (WAM–T147351): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.     FIGURE 11. Habitus images of preserved holotype  <b>Maratus</b> combustus   sp. nov.  (WAM–T147351): A, dorsal view; B, ventral view; C, anterior",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271047,
				"treatmentId": "D17A87C7D5064856FC0899F49895C54B",
				"treatmentTitle": "Maratus bubo Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "bubo",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Emergent or second instar   <b>Maratus</b> bubo   . This is the first instar to emerge from the brood sac.             Figure 42. Four penultimate female (1-6) and four penultimate male (7-12)   <b>Maratus</b> bubo   .          Courtship (      Figures 43 -44  ,    45 : 1 ). Courtship display by the male  <b>Maratus</b> bubo  is similar to that previously",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271048,
				"treatmentId": "D17A87C7D50B486DFC3499F498E9C5B4",
				"treatmentTitle": "Maratus australis Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "australis",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Five adult female  <b>Maratus</b> australis  .             Figure 27. Views of an adult female  <b>Maratus</b> australis  . 3, Note the sharp definition of the tapering median thoracic band on a black background.             Figure 28. Ventral views of two adult female  <b>Maratus</b> australis  .             Figure 29. Adult female  <b>Maratus</b> australis  specimens in alcohol. 8-11",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271049,
				"treatmentId": "D17A87C7D51A487EFC0C99F49EFAC477",
				"treatmentTitle": "Maratus albus Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "albus",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Four adult male  <b>Maratus</b> albus  from Eyre Bird Observatory in alcohol. 1-4, Holotype.             Figure 5. Medial to lateral views of the left pedipalp of five adult male  <b>Maratus</b> albus  from Eyre Bird Observatory, all types. 1- 5, Holotype.             Figure 6. Frontal views of two adult male  <b>Maratus</b> albus  from",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271050,
				"treatmentId": "D17A87C7D52F4833FC2199F49DDCC534",
				"treatmentTitle": "Maratus tessellatus Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "tessellatus",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Four different female  <b>Maratus</b> tessellatus  .             Figure 65. Views of a female  <b>Maratus</b> tessellatus  .             Figure 66. Ventral views of four female  <b>Maratus</b> tessellatus  .        1 mm 1 mm 1 mm 1 mm 1 mm 1 mm        1 mm 1 mm        1 mm        1 mm        1 mm 1 mm             Figure 67. Three female",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271051,
				"treatmentId": "D17A87C7D5334841FC3E99F498C6C5D1",
				"treatmentTitle": "Maratus lobatus Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "lobatus",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Three different female  <b>Maratus</b> lobatus  in alcohol.             Figure 55. Female  <b>Maratus</b> lobatus  in alcohol. 9-13, Detail of epigynum of five different females. Note variability in width of septum and sclerotization of ducts visible behind the posterior portion of each fenestra.             Figure 56. Female  <b>Maratus</b> lobatus  . 2, Detail of face",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271052,
				"treatmentId": "D17A87C7D542482EFC0099F499AAC127",
				"treatmentTitle": "Maratus vultus Otto & Hill, 2016, new specIes",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "vultus",
				"status": "new specIes",
				"taxonomicNameLabel": "new specIes",
				"rank": "species",
				"context": "Display positions of a male  <b>Maratus</b> vultus  (♂ #1, holotype) in front of a female  <b>Maratus</b> fimbriatus  .         Habitat and distribution (      Figure 109  , for map see      Figure 1  ). Presently  <b>Maratus</b> vultus  is known from the type locality at Point Ann in Fitzgerald River National Park, WA and from Esperance, WA, where it",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271053,
				"treatmentId": "D17A87C7D5584829FC0D99F49FF5C127",
				"treatmentTitle": "Maratus vespa Otto & Hill, 2016, new species",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "vespa",
				"status": "new species",
				"taxonomicNameLabel": "new species",
				"rank": "species",
				"context": "Four different female  <b>Maratus</b> vespa  in alcohol.             Figure 90. Female  <b>Maratus</b> vespa  in alcohol.             Figure 91. Ventral views of six living female  <b>Maratus</b> vespa  .             Figure 92. Ventral views of the epigynum of six female  <b>Maratus</b> vespa  , in alcohol. 1-2, Ventral view of dissected epigynum. 3, Dorsal (interior) view of",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 271054,
				"treatmentId": "D17A87C7D57B4812FFF099F79CBFC18D",
				"treatmentTitle": "Maratus",
				"articleDoi": "10.5281/zenodo.270111",
				"zenodoDep": "270111",
				"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
				"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
				"publicationDate": "",
				"journalTitle": "Peckhamia",
				"journalYear": "2016",
				"journalVolume": "141",
				"journalIssue": "1",
				"pages": "1–101",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "genus",
				"context": "Otto & Hill 2012 c  , 2012 e, 2016 b         <b>Maratus</b> vultus Otto & HIll 2016          <b>Maratus</b> vultus Otto & Hill 2016 b          calcitrans group          <b>Maratus</b> calcitrans  Otto & HIll 2012         <b>Maratus</b> calcitrans  Otto & Hill 2012 d  <b>Maratus</b> digitatus  Otto & HIll 2012         <b>Maratus</b> digitatus  Otto & Hill 2012 d         <b>Maratus</b> jactatus  Otto & HIll 2015         <b>Maratus</b> jactatus",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275701,
				"treatmentId": "D709975BC52956782DB3FD0E36B5FE66",
				"treatmentTitle": "Maratus ottoi Baehr & Whyte, 2016, sp. nov.",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Baehr & Whyte",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "ottoi",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "The specific name is a patronym in honour of Dr Jürgen Otto, one of Australia’s most accomplished  <b>Maratus</b>  experts.        Diagnosis.  M. ottoi  is closely related to  M. eliasi  sharing a nearly identical prosomal colour pattern (   Figs 12 A, 13A) and a similar embolic disc (   Figs 11 A, B).  M",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275702,
				"treatmentId": "D709975BC52D56782DB3FE5335ABFCFD",
				"treatmentTitle": "Maratus pavonis",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "pavonis",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "The  <b>Maratus</b> pavonis  group        (   FIGURES 15 C, F, I, 16A ‒I)        This group contains those species with an embolic disc which has a broad smooth rim and a broad bent embolic ridge with the embolic opening at the frontal end (   Fig. 15 F). The lateral process of the embolic disc",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275703,
				"treatmentId": "D709975BC52D567B2DB3FCD33666FEF3",
				"treatmentTitle": "Maratus pavonis var. nornalup",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "pavonis",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "variety",
				"context": "Dunn, 1947  , 1957  <b>Maratus</b> pavonis , Żabka, 1991  ;       <b>Maratus</b> pavonis Otto & Hill, 2014b  .          Material examined.  1 male (WAM-T136127) from Australia , Western Australia Nornalup Inlet , 35°01’S , 116°44’E , B. & M. Baehr ,  1‒2. Dec. 1987  , hand coll.         Etymology. The var. name refers to the location Nornalup Inlet.        Diagnosis",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275704,
				"treatmentId": "D709975BC52F567A2DB3FC1D3037F90B",
				"treatmentTitle": "Maratus volans O. Pickard-Cambridge 1874",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "O. Pickard-Cambridge",
				"authorityYear": "1874",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "volans",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "4         <b>Maratus</b> amoenus  Karsch, 1878d : 28   .         Saitis volans :  Simon 1901 : 559   , 563, figs 677‒679;  Butler 1933 : 291  , pl. 17, fig. 6;  Prószyński 1984 : 126  (m).         <b>Maratus</b> amoenus  Żabka, 1987 : 479   , fig. 67‒69 (Dm; N.B.: a primary junior homonym and an objective junior synonym of  M. amoenus Karsch",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275705,
				"treatmentId": "D709975BC52F567A2DB3FD173642FCD1",
				"treatmentTitle": "Maratus volans",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "volans",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "The  <b>Maratus</b> volans  group        (   FIGURES 15 A, D, G)        Otto & Hill (2014a) described the  <b>Maratus</b> volans  group (  M. pardus  and  M. volans  ) as having a wide fringe at the sides of the opisthosoma and similar courtship displays.",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275706,
				"treatmentId": "D709975BC52F567A2DB3FF1830D3FDAB",
				"treatmentTitle": "Maratus speciosus O. Pickard-Cambridge 1874",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "O. Pickard-Cambridge",
				"authorityYear": "1874",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "speciosus",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "You tube Peacock Spider 7  ( <b>Maratus</b> speciosus )  (https://www.youtube.com/watch?v=d_yYC5r8xMI).",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275707,
				"treatmentId": "D709975BC53056642DB3F8A63683FE4C",
				"treatmentTitle": "Maratus anomalus Karsch 1878",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Karsch",
				"authorityYear": "1878",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "anomalus",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "<b>Maratus</b> anomalus ( Karsch, 1878 )         (   FIGURE 7 A, D, G)          Lycidas anomalus  Karsch, 1878d : 26   ;  Prószyński 1984a : 159  (removed m from S of  Saitis nigriceps  );  Żabka, 1987 : 471  , figs 50‒51.         <b>Maratus</b> anomalus  Otto & Hill, 2012a : 23   , figs. 28.1‒12, 29.1‒4, 30.1‒8, 31.1‒8, 32",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275708,
				"treatmentId": "D709975BC53056652DB3FA11313CF938",
				"treatmentTitle": "Maratus anomalus",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "anomalus",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "The  <b>Maratus</b> anomalus  group        (   FIGURES 7 A ‒I, 8A ‒N, 10A ‒I)        This group contains species with a pair of large patches of white setae on the posterior sides of the prosoma (   Figs 8 A, E, 10B), with an embolic disc which has a smooth narrow front with a retrobasal",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275709,
				"treatmentId": "D709975BC53256632DB3F9F13437FF16",
				"treatmentTitle": "Maratus michaelorum Baehr & Whyte, 2016, sp. nov.",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Baehr & Whyte",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "michaelorum",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "The specific name is a patronym in honour of Michael Duncan and Michael Doe, who are experts at finding new members of the  <b>Maratus</b> anomalus  group mostly in “tussock grass” and who provided excellent live photography for this paper.           FIGURE 8 (A ‒N).  <b>Maratus</b> julianneae Baehr & Whyte  ,  sp. nov.  male",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275710,
				"treatmentId": "D709975BC53256672DB3FF18314DF9C5",
				"treatmentTitle": "Maratus julianneae Baehr & Whyte, 2016, sp. nov.",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Baehr & Whyte",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "julianneae",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "The specific name is a patronym in honour of Julianne Waldock, for her contributions to  <b>Maratus</b>  systematics over more than two decades. She also provided excellent support for Madeline Girard in finding  <b>Maratus</b>  localities.        Diagnosis. This species belongs to the  <b>Maratus</b> anomalus  group, sharing a pair of large patches of",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275711,
				"treatmentId": "D709975BC53656632DB3FC9136B1FB53",
				"treatmentTitle": "Maratus digitatus Otto & Hill 2012",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Otto & Hill",
				"authorityYear": "2012",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "digitatus",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "<b>Maratus</b> digitatus Otto & Hill, 2012         (   FIGURES 11 C, F, I)          <b>Maratus</b> digitatus  Otto & Hill, 2012b : 10   , figs 12‒27. Type locality: Mount Kaputar near Narrabri, northern New South Wales.           Material examined.  AUSTRALIA : 2 males (QM-S47268), south-east Queensland , Nipping Gully , site 5, Rainforest , 25°42’S , 151°26’E",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275712,
				"treatmentId": "D709975BC53656632DB3FEC337D6FD25",
				"treatmentTitle": "Maratus digitatus",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "digitatus",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "The  <b>Maratus</b> digitatus  group        (   FIGURES 11 A ‒I, 12A ‒I, 13A ‒I)        This group contains species with small flaps, displaying with one leg to one side and with inflated spinnerets (J. Otto, pers. comm.). They have an embolic disc with a broad smooth front and a broad spatulate embolic tip",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275713,
				"treatmentId": "D709975BC536567C2DB3FA803788FDAE",
				"treatmentTitle": "Maratus eliasi Baehr & Whyte, 2016, sp. nov.",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Baehr & Whyte",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "eliasi",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "37 as  <b>Maratus</b> cf. digitatus  ) sharing a nearly identical prosomal colour pattern and in having a larger pair of semicircular, iridescent, flaps which are uniformly dark green in  M. digitatus  .       M. eliasi  can be separated from  M. digitatus  by its opisthosomal colour pattern (golden and striped flaps) (   Fig. 12 A",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275714,
				"treatmentId": "D709975BC539566C2DB3F91A34FDF86B",
				"treatmentTitle": "Maratus",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "genus",
				"context": "The  <b>Maratus</b>  species groups        Species groups suggested by Waldock (2013) and Otto & Hill (2014b , 2015 ) take into account differentiation of abdominal patterns and lateral ornamentation, inflatable spinnerets, and behaviour, especially male courtship.      In this paper the male embolic discs of all examined species, studied by Scanning Electron Microscopy (SEM), revealed",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275715,
				"treatmentId": "D709975BC539566C2DB3FD7B373DF9AF",
				"treatmentTitle": "Maratus Karsch 1878",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Karsch",
				"authorityYear": "1878",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "genus",
				"context": "Genus  <b>Maratus</b> Karsch, 1878             <b>Maratus</b>  Karsch, 1878 : 27   . Type species designated by monotypy:  <b>Maratus</b> amabilis Karsch, 1878  , in Bonnet, 1957: 2713.        The endemic Australian Jumping spider genus  <b>Maratus</b>  belongs to the  Saitis  clade together with the salticid genera  Saitis  ,  Jotus  ,  Prostheclina  ,  Hypoblemum  , ‘Lycidas’ ,  Maileus  ,  Barraina  and possibly  Margaromma ( Zhang & Maddison",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275716,
				"treatmentId": "D709975BC53A566E2DB3FC653752FF16",
				"treatmentTitle": "Maratus kiwirrkurra Baehr & Whyte, 2016, sp. nov.",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Baehr & Whyte",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "kiwirrkurra",
				"status": "sp. nov.",
				"taxonomicNameLabel": "sp. nov.",
				"rank": "species",
				"context": "This small species belongs to the  <b>Maratus</b> chrysomelas  group, having a wide rimmed embolic disc covered with frontal ridges. There is no retrolateral process of the embolic disc.  M. kiwirrkurra  can be separated from other species of this group by the prosoma and opisthosoma being covered with cinnamon and white",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275717,
				"treatmentId": "D709975BC53A566F2DB3FDC937A8FC79",
				"treatmentTitle": "Maratus chrysomelas Simon 1909",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "Simon",
				"authorityYear": "1909",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "chrysomelas",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "<b>Maratus</b> chrysomelas ( Simon, 1909 )         (   FIGURES 1 B, E, H)          Habrocestum chrysomelas  Simon, 1909 : 201   .         Lycidas chrysomelas :  Żabka, 1987 : 457   , figs 19‒22;  Waldock, 2002 : 228  , figs 1‒10.           Material examined.  MALE (QM-S96329) from Australia , central Queensland , Emerald , 23°31’S , 148°09’E , L. Sanders ,  26 Sep. 2015  , hand",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			},
			{
				"id": 275718,
				"treatmentId": "D709975BC53A566F2DB3FF173033FE1C",
				"treatmentTitle": "Maratus chrysomelas",
				"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
				"zenodoDep": "255783",
				"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
				"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
				"publicationDate": "",
				"journalTitle": "Zootaxa",
				"journalYear": "2016",
				"journalVolume": "4154",
				"journalIssue": "5",
				"pages": "501–525",
				"authorityName": "",
				"authorityYear": "",
				"kingdom": "Animalia",
				"phylum": "Arthropoda",
				"order": "Araneae",
				"family": "Salticidae",
				"genus": "Maratus",
				"species": "chrysomelas",
				"status": "",
				"taxonomicNameLabel": "",
				"rank": "species",
				"context": "The  <b>Maratus</b> chrysomelas  group        (   FIGURES 1 A, B, D, E, G, H)        Otto & Hill (2016a) described the  <b>Maratus</b> chrysomelas  group (  M. chrysomelas  and  M. nigromaculatus  ) as having a wide fringe at the sides of the opisthosoma and similar courtship displays. We find also this group contains species which have an",
				"_links": {
					"self": {
						"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
					}
				}
			}
		],
		"nextid": 275718,
		"from": 1,
		"to": 30,
		"previd": 0,
		"prevpage": 0,
		"nextpage": 2,
		"facets": {
			"journalVolume": [
				{
					"journalVolume": "112",
					"c": 7
				},
				{
					"journalVolume": "141",
					"c": 8
				},
				{
					"journalVolume": "4000",
					"c": 1
				},
				{
					"journalVolume": "4154",
					"c": 20
				},
				{
					"journalVolume": "4564",
					"c": 4
				}
			],
			"journalTitle": [
				{
					"journalTitle": "Peckhamia",
					"c": 15
				},
				{
					"journalTitle": "Zootaxa",
					"c": 25
				}
			],
			"journalYear": [
				{
					"journalYear": "2014",
					"c": 7
				},
				{
					"journalYear": "2015",
					"c": 1
				},
				{
					"journalYear": "2016",
					"c": 28
				},
				{
					"journalYear": "2019",
					"c": 4
				}
			],
			"kingdom": [
				{
					"kingdom": "Animalia",
					"c": 39
				}
			],
			"phylum": [
				{
					"phylum": "Arthropoda",
					"c": 39
				}
			],
			"order": [
				{
					"order": "Araneae",
					"c": 39
				}
			],
			"family": [
				{
					"family": "Salticidae",
					"c": 39
				}
			],
			"genus": [
				{
					"genus": "Maratus",
					"c": 38
				},
				{
					"genus": "Tauala",
					"c": 1
				}
			],
			"status": [
				{
					"status": "new specIes",
					"c": 1
				},
				{
					"status": "new species",
					"c": 7
				},
				{
					"status": "sp. nov.",
					"c": 10
				}
			],
			"rank": [
				{
					"rank": "genus",
					"c": 5
				},
				{
					"rank": "species",
					"c": 33
				},
				{
					"rank": "variety",
					"c": 1
				}
			],
			"species": [
				{
					"species": "albus",
					"c": 1
				},
				{
					"species": "anomalus",
					"c": 2
				},
				{
					"species": "aquilus",
					"c": 1
				},
				{
					"species": "australis",
					"c": 1
				},
				{
					"species": "avibus",
					"c": 1
				},
				{
					"species": "bubo",
					"c": 1
				},
				{
					"species": "chrysomelas",
					"c": 2
				},
				{
					"species": "combustus",
					"c": 1
				},
				{
					"species": "digitatus",
					"c": 2
				},
				{
					"species": "eliasi",
					"c": 1
				},
				{
					"species": "felinus",
					"c": 1
				},
				{
					"species": "fimbriatus",
					"c": 1
				},
				{
					"species": "julianneae",
					"c": 1
				},
				{
					"species": "karrie",
					"c": 1
				},
				{
					"species": "kiwirrkurra",
					"c": 1
				},
				{
					"species": "licunxini",
					"c": 1
				},
				{
					"species": "lobatus",
					"c": 1
				},
				{
					"species": "melindae",
					"c": 1
				},
				{
					"species": "michaelorum",
					"c": 1
				},
				{
					"species": "mungaich",
					"c": 1
				},
				{
					"species": "ottoi",
					"c": 2
				},
				{
					"species": "pavonis",
					"c": 2
				},
				{
					"species": "sarahae",
					"c": 1
				},
				{
					"species": "speciosus",
					"c": 1
				},
				{
					"species": "tessellatus",
					"c": 1
				},
				{
					"species": "vespa",
					"c": 1
				},
				{
					"species": "volans",
					"c": 2
				},
				{
					"species": "vultus",
					"c": 1
				}
			],
			"collectionCode": [
				{
					"collectionCode": "MALE",
					"c": 17
				},
				{
					"collectionCode": "NSW",
					"c": 2
				},
				{
					"collectionCode": "Western Australian Museum, Perth",
					"c": 1
				}
			]
		},
		"stats": {
			"specimens": [
				{
					"Sum(specimenCount)": 78
				}
			],
			"male specimens": [
				{
					"Sum(specimenCountMale)": null
				}
			],
			"female specimens": [
				{
					"Sum(specimenCountFemale)": null
				}
			],
			"treatments with specimens": [
				{
					"Count(DISTINCT treatments.treatmentId)": 20
				}
			],
			"treatments with male specimens": [
				{
					"Count(DISTINCT treatments.treatmentId)": 0
				}
			],
			"treatments with female specimens": [
				{
					"Count(DISTINCT treatments.treatmentId)": 0
				}
			],
			"figure citations": [
				{
					"Count(figureCitationId)": 301
				}
			]
		}
	},
	"cached": {
		"item": {
			"num-of-records": 40,
			"search-criteria": {
				"facets": "true",
				"page": "1",
				"q": "Maratus",
				"size": "30",
				"sortBy": "treatmentId:ASC",
				"stats": "true",
				"resource": "treatments",
				"limit": 30,
				"offset": 0
			},
			"_links": {
				"self": {
					"href": "https://zenodeo.punkish.org/treatments?facets=true&page=1&q=Maratus&resource=treatments&size=30&sortBy=treatmentId:ASC&stats=true"
				}
			},
			"records": [
				{
					"id": 96939,
					"treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D",
					"treatmentTitle": "Maratus felinus Schubert, 2019, sp. nov.",
					"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
					"zenodoDep": "2588669",
					"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
					"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
					"publicationDate": "2019-03-05",
					"journalTitle": "Zootaxa",
					"journalYear": "2019",
					"journalVolume": "4564",
					"journalIssue": "1",
					"pages": "81–100",
					"authorityName": "Schubert",
					"authorityYear": "2019",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "felinus",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "Habitus images of living holotype  <b>Maratus</b> felinus   sp. nov.  (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.     FIGURE 18. Habitus images of preserved holotype  <b>Maratus</b> felinus   sp. nov.  (WAM–T147353): A, dorsal view; B, ventral view; C, anterior",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 96940,
					"treatmentId": "03FE87F49708FF92FF15F958FC94BB2E",
					"treatmentTitle": "Maratus aquilus Schubert, 2019, sp. nov.",
					"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
					"zenodoDep": "2588669",
					"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
					"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
					"publicationDate": "2019-03-05",
					"journalTitle": "Zootaxa",
					"journalYear": "2019",
					"journalVolume": "4564",
					"journalIssue": "1",
					"pages": "81–100",
					"authorityName": "Schubert",
					"authorityYear": "2019",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "aquilus",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "Living male paratype  <b>Maratus</b> aquilus   sp. nov.  ,  M. combustus   sp. nov.  , and  M. felinus   sp. nov.  performing courtship display to nearby female: A, Courtship display of male  <b>Maratus</b> aquilus   sp. nov.  ; B, courtship display of  <b>Maratus</b> combustus   sp. nov.  ; C, courtship display  of <b>Maratus</b> felinus  sp. nov.     Diagnosis. This species",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 96941,
					"treatmentId": "03FE87F49708FF94FF15F999FEA2BBAD",
					"treatmentTitle": "Maratus Karsch 1878",
					"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
					"zenodoDep": "2588669",
					"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
					"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
					"publicationDate": "2019-03-05",
					"journalTitle": "Zootaxa",
					"journalYear": "2019",
					"journalVolume": "4564",
					"journalIssue": "1",
					"pages": "81–100",
					"authorityName": "Karsch",
					"authorityYear": "1878",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "genus",
					"context": "Genus  <b>Maratus</b> Karsch, 1878          <b>Maratus</b>  Karsch, 1878 : 27   . Type species, by monotypy:  <b>Maratus</b> amabilis Karsch, 1878  , in   Bonnet, 1957: 2713.",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 96942,
					"treatmentId": "03FE87F4970EFF98FF15F9CBFDB7BE25",
					"treatmentTitle": "Maratus combustus Schubert, 2019, sp. nov.",
					"articleDoi": "https://doi.org/10.11646/zootaxa.4564.1.3",
					"zenodoDep": "2588669",
					"zoobank": "B8991FC7-399B-4B00-B968-D3BC44F32020",
					"articleTitle": "Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)",
					"publicationDate": "2019-03-05",
					"journalTitle": "Zootaxa",
					"journalYear": "2019",
					"journalVolume": "4564",
					"journalIssue": "1",
					"pages": "81–100",
					"authorityName": "Schubert",
					"authorityYear": "2019",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "combustus",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "Habitus images of living holotype  <b>Maratus</b> combustus   sp. nov.  (WAM–T147351): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.     FIGURE 11. Habitus images of preserved holotype  <b>Maratus</b> combustus   sp. nov.  (WAM–T147351): A, dorsal view; B, ventral view; C, anterior",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271047,
					"treatmentId": "D17A87C7D5064856FC0899F49895C54B",
					"treatmentTitle": "Maratus bubo Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "bubo",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Emergent or second instar   <b>Maratus</b> bubo   . This is the first instar to emerge from the brood sac.             Figure 42. Four penultimate female (1-6) and four penultimate male (7-12)   <b>Maratus</b> bubo   .          Courtship (      Figures 43 -44  ,    45 : 1 ). Courtship display by the male  <b>Maratus</b> bubo  is similar to that previously",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271048,
					"treatmentId": "D17A87C7D50B486DFC3499F498E9C5B4",
					"treatmentTitle": "Maratus australis Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "australis",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Five adult female  <b>Maratus</b> australis  .             Figure 27. Views of an adult female  <b>Maratus</b> australis  . 3, Note the sharp definition of the tapering median thoracic band on a black background.             Figure 28. Ventral views of two adult female  <b>Maratus</b> australis  .             Figure 29. Adult female  <b>Maratus</b> australis  specimens in alcohol. 8-11",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271049,
					"treatmentId": "D17A87C7D51A487EFC0C99F49EFAC477",
					"treatmentTitle": "Maratus albus Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "albus",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Four adult male  <b>Maratus</b> albus  from Eyre Bird Observatory in alcohol. 1-4, Holotype.             Figure 5. Medial to lateral views of the left pedipalp of five adult male  <b>Maratus</b> albus  from Eyre Bird Observatory, all types. 1- 5, Holotype.             Figure 6. Frontal views of two adult male  <b>Maratus</b> albus  from",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271050,
					"treatmentId": "D17A87C7D52F4833FC2199F49DDCC534",
					"treatmentTitle": "Maratus tessellatus Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "tessellatus",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Four different female  <b>Maratus</b> tessellatus  .             Figure 65. Views of a female  <b>Maratus</b> tessellatus  .             Figure 66. Ventral views of four female  <b>Maratus</b> tessellatus  .        1 mm 1 mm 1 mm 1 mm 1 mm 1 mm        1 mm 1 mm        1 mm        1 mm        1 mm 1 mm             Figure 67. Three female",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271051,
					"treatmentId": "D17A87C7D5334841FC3E99F498C6C5D1",
					"treatmentTitle": "Maratus lobatus Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "lobatus",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Three different female  <b>Maratus</b> lobatus  in alcohol.             Figure 55. Female  <b>Maratus</b> lobatus  in alcohol. 9-13, Detail of epigynum of five different females. Note variability in width of septum and sclerotization of ducts visible behind the posterior portion of each fenestra.             Figure 56. Female  <b>Maratus</b> lobatus  . 2, Detail of face",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271052,
					"treatmentId": "D17A87C7D542482EFC0099F499AAC127",
					"treatmentTitle": "Maratus vultus Otto & Hill, 2016, new specIes",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "vultus",
					"status": "new specIes",
					"taxonomicNameLabel": "new specIes",
					"rank": "species",
					"context": "Display positions of a male  <b>Maratus</b> vultus  (♂ #1, holotype) in front of a female  <b>Maratus</b> fimbriatus  .         Habitat and distribution (      Figure 109  , for map see      Figure 1  ). Presently  <b>Maratus</b> vultus  is known from the type locality at Point Ann in Fitzgerald River National Park, WA and from Esperance, WA, where it",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271053,
					"treatmentId": "D17A87C7D5584829FC0D99F49FF5C127",
					"treatmentTitle": "Maratus vespa Otto & Hill, 2016, new species",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "vespa",
					"status": "new species",
					"taxonomicNameLabel": "new species",
					"rank": "species",
					"context": "Four different female  <b>Maratus</b> vespa  in alcohol.             Figure 90. Female  <b>Maratus</b> vespa  in alcohol.             Figure 91. Ventral views of six living female  <b>Maratus</b> vespa  .             Figure 92. Ventral views of the epigynum of six female  <b>Maratus</b> vespa  , in alcohol. 1-2, Ventral view of dissected epigynum. 3, Dorsal (interior) view of",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 271054,
					"treatmentId": "D17A87C7D57B4812FFF099F79CBFC18D",
					"treatmentTitle": "Maratus",
					"articleDoi": "10.5281/zenodo.270111",
					"zenodoDep": "270111",
					"zoobank": "urn:lsid:zoobank.org:pub:F1BC047C-7963-491E-A55C-3D1313B58510",
					"articleTitle": "Seven new peacock spiders from Western Australia and South Australia (Araneae: Salticidae: Euophryini: Maratus)",
					"publicationDate": "",
					"journalTitle": "Peckhamia",
					"journalYear": "2016",
					"journalVolume": "141",
					"journalIssue": "1",
					"pages": "1–101",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "genus",
					"context": "Otto & Hill 2012 c  , 2012 e, 2016 b         <b>Maratus</b> vultus Otto & HIll 2016          <b>Maratus</b> vultus Otto & Hill 2016 b          calcitrans group          <b>Maratus</b> calcitrans  Otto & HIll 2012         <b>Maratus</b> calcitrans  Otto & Hill 2012 d  <b>Maratus</b> digitatus  Otto & HIll 2012         <b>Maratus</b> digitatus  Otto & Hill 2012 d         <b>Maratus</b> jactatus  Otto & HIll 2015         <b>Maratus</b> jactatus",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275701,
					"treatmentId": "D709975BC52956782DB3FD0E36B5FE66",
					"treatmentTitle": "Maratus ottoi Baehr & Whyte, 2016, sp. nov.",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Baehr & Whyte",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "ottoi",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "The specific name is a patronym in honour of Dr Jürgen Otto, one of Australia’s most accomplished  <b>Maratus</b>  experts.        Diagnosis.  M. ottoi  is closely related to  M. eliasi  sharing a nearly identical prosomal colour pattern (   Figs 12 A, 13A) and a similar embolic disc (   Figs 11 A, B).  M",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275702,
					"treatmentId": "D709975BC52D56782DB3FE5335ABFCFD",
					"treatmentTitle": "Maratus pavonis",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "pavonis",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "The  <b>Maratus</b> pavonis  group        (   FIGURES 15 C, F, I, 16A ‒I)        This group contains those species with an embolic disc which has a broad smooth rim and a broad bent embolic ridge with the embolic opening at the frontal end (   Fig. 15 F). The lateral process of the embolic disc",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275703,
					"treatmentId": "D709975BC52D567B2DB3FCD33666FEF3",
					"treatmentTitle": "Maratus pavonis var. nornalup",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "pavonis",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "variety",
					"context": "Dunn, 1947  , 1957  <b>Maratus</b> pavonis , Żabka, 1991  ;       <b>Maratus</b> pavonis Otto & Hill, 2014b  .          Material examined.  1 male (WAM-T136127) from Australia , Western Australia Nornalup Inlet , 35°01’S , 116°44’E , B. & M. Baehr ,  1‒2. Dec. 1987  , hand coll.         Etymology. The var. name refers to the location Nornalup Inlet.        Diagnosis",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275704,
					"treatmentId": "D709975BC52F567A2DB3FC1D3037F90B",
					"treatmentTitle": "Maratus volans O. Pickard-Cambridge 1874",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "O. Pickard-Cambridge",
					"authorityYear": "1874",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "volans",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "4         <b>Maratus</b> amoenus  Karsch, 1878d : 28   .         Saitis volans :  Simon 1901 : 559   , 563, figs 677‒679;  Butler 1933 : 291  , pl. 17, fig. 6;  Prószyński 1984 : 126  (m).         <b>Maratus</b> amoenus  Żabka, 1987 : 479   , fig. 67‒69 (Dm; N.B.: a primary junior homonym and an objective junior synonym of  M. amoenus Karsch",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275705,
					"treatmentId": "D709975BC52F567A2DB3FD173642FCD1",
					"treatmentTitle": "Maratus volans",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "volans",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "The  <b>Maratus</b> volans  group        (   FIGURES 15 A, D, G)        Otto & Hill (2014a) described the  <b>Maratus</b> volans  group (  M. pardus  and  M. volans  ) as having a wide fringe at the sides of the opisthosoma and similar courtship displays.",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275706,
					"treatmentId": "D709975BC52F567A2DB3FF1830D3FDAB",
					"treatmentTitle": "Maratus speciosus O. Pickard-Cambridge 1874",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "O. Pickard-Cambridge",
					"authorityYear": "1874",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "speciosus",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "You tube Peacock Spider 7  ( <b>Maratus</b> speciosus )  (https://www.youtube.com/watch?v=d_yYC5r8xMI).",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275707,
					"treatmentId": "D709975BC53056642DB3F8A63683FE4C",
					"treatmentTitle": "Maratus anomalus Karsch 1878",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Karsch",
					"authorityYear": "1878",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "anomalus",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "<b>Maratus</b> anomalus ( Karsch, 1878 )         (   FIGURE 7 A, D, G)          Lycidas anomalus  Karsch, 1878d : 26   ;  Prószyński 1984a : 159  (removed m from S of  Saitis nigriceps  );  Żabka, 1987 : 471  , figs 50‒51.         <b>Maratus</b> anomalus  Otto & Hill, 2012a : 23   , figs. 28.1‒12, 29.1‒4, 30.1‒8, 31.1‒8, 32",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275708,
					"treatmentId": "D709975BC53056652DB3FA11313CF938",
					"treatmentTitle": "Maratus anomalus",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "anomalus",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "The  <b>Maratus</b> anomalus  group        (   FIGURES 7 A ‒I, 8A ‒N, 10A ‒I)        This group contains species with a pair of large patches of white setae on the posterior sides of the prosoma (   Figs 8 A, E, 10B), with an embolic disc which has a smooth narrow front with a retrobasal",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275709,
					"treatmentId": "D709975BC53256632DB3F9F13437FF16",
					"treatmentTitle": "Maratus michaelorum Baehr & Whyte, 2016, sp. nov.",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Baehr & Whyte",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "michaelorum",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "The specific name is a patronym in honour of Michael Duncan and Michael Doe, who are experts at finding new members of the  <b>Maratus</b> anomalus  group mostly in “tussock grass” and who provided excellent live photography for this paper.           FIGURE 8 (A ‒N).  <b>Maratus</b> julianneae Baehr & Whyte  ,  sp. nov.  male",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275710,
					"treatmentId": "D709975BC53256672DB3FF18314DF9C5",
					"treatmentTitle": "Maratus julianneae Baehr & Whyte, 2016, sp. nov.",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Baehr & Whyte",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "julianneae",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "The specific name is a patronym in honour of Julianne Waldock, for her contributions to  <b>Maratus</b>  systematics over more than two decades. She also provided excellent support for Madeline Girard in finding  <b>Maratus</b>  localities.        Diagnosis. This species belongs to the  <b>Maratus</b> anomalus  group, sharing a pair of large patches of",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275711,
					"treatmentId": "D709975BC53656632DB3FC9136B1FB53",
					"treatmentTitle": "Maratus digitatus Otto & Hill 2012",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Otto & Hill",
					"authorityYear": "2012",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "digitatus",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "<b>Maratus</b> digitatus Otto & Hill, 2012         (   FIGURES 11 C, F, I)          <b>Maratus</b> digitatus  Otto & Hill, 2012b : 10   , figs 12‒27. Type locality: Mount Kaputar near Narrabri, northern New South Wales.           Material examined.  AUSTRALIA : 2 males (QM-S47268), south-east Queensland , Nipping Gully , site 5, Rainforest , 25°42’S , 151°26’E",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275712,
					"treatmentId": "D709975BC53656632DB3FEC337D6FD25",
					"treatmentTitle": "Maratus digitatus",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "digitatus",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "The  <b>Maratus</b> digitatus  group        (   FIGURES 11 A ‒I, 12A ‒I, 13A ‒I)        This group contains species with small flaps, displaying with one leg to one side and with inflated spinnerets (J. Otto, pers. comm.). They have an embolic disc with a broad smooth front and a broad spatulate embolic tip",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275713,
					"treatmentId": "D709975BC536567C2DB3FA803788FDAE",
					"treatmentTitle": "Maratus eliasi Baehr & Whyte, 2016, sp. nov.",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Baehr & Whyte",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "eliasi",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "37 as  <b>Maratus</b> cf. digitatus  ) sharing a nearly identical prosomal colour pattern and in having a larger pair of semicircular, iridescent, flaps which are uniformly dark green in  M. digitatus  .       M. eliasi  can be separated from  M. digitatus  by its opisthosomal colour pattern (golden and striped flaps) (   Fig. 12 A",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275714,
					"treatmentId": "D709975BC539566C2DB3F91A34FDF86B",
					"treatmentTitle": "Maratus",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "genus",
					"context": "The  <b>Maratus</b>  species groups        Species groups suggested by Waldock (2013) and Otto & Hill (2014b , 2015 ) take into account differentiation of abdominal patterns and lateral ornamentation, inflatable spinnerets, and behaviour, especially male courtship.      In this paper the male embolic discs of all examined species, studied by Scanning Electron Microscopy (SEM), revealed",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275715,
					"treatmentId": "D709975BC539566C2DB3FD7B373DF9AF",
					"treatmentTitle": "Maratus Karsch 1878",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Karsch",
					"authorityYear": "1878",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "genus",
					"context": "Genus  <b>Maratus</b> Karsch, 1878             <b>Maratus</b>  Karsch, 1878 : 27   . Type species designated by monotypy:  <b>Maratus</b> amabilis Karsch, 1878  , in Bonnet, 1957: 2713.        The endemic Australian Jumping spider genus  <b>Maratus</b>  belongs to the  Saitis  clade together with the salticid genera  Saitis  ,  Jotus  ,  Prostheclina  ,  Hypoblemum  , ‘Lycidas’ ,  Maileus  ,  Barraina  and possibly  Margaromma ( Zhang & Maddison",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275716,
					"treatmentId": "D709975BC53A566E2DB3FC653752FF16",
					"treatmentTitle": "Maratus kiwirrkurra Baehr & Whyte, 2016, sp. nov.",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Baehr & Whyte",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "kiwirrkurra",
					"status": "sp. nov.",
					"taxonomicNameLabel": "sp. nov.",
					"rank": "species",
					"context": "This small species belongs to the  <b>Maratus</b> chrysomelas  group, having a wide rimmed embolic disc covered with frontal ridges. There is no retrolateral process of the embolic disc.  M. kiwirrkurra  can be separated from other species of this group by the prosoma and opisthosoma being covered with cinnamon and white",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275717,
					"treatmentId": "D709975BC53A566F2DB3FDC937A8FC79",
					"treatmentTitle": "Maratus chrysomelas Simon 1909",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "Simon",
					"authorityYear": "1909",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "chrysomelas",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "<b>Maratus</b> chrysomelas ( Simon, 1909 )         (   FIGURES 1 B, E, H)          Habrocestum chrysomelas  Simon, 1909 : 201   .         Lycidas chrysomelas :  Żabka, 1987 : 457   , figs 19‒22;  Waldock, 2002 : 228  , figs 1‒10.           Material examined.  MALE (QM-S96329) from Australia , central Queensland , Emerald , 23°31’S , 148°09’E , L. Sanders ,  26 Sep. 2015  , hand",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				},
				{
					"id": 275718,
					"treatmentId": "D709975BC53A566F2DB3FF173033FE1C",
					"treatmentTitle": "Maratus chrysomelas",
					"articleDoi": "http://doi.org/10.11646/zootaxa.4154.5.1",
					"zenodoDep": "255783",
					"zoobank": "9C689664-C36A-46F8-B106-6EF6D18B1D50",
					"articleTitle": "The Peacock Spiders (Araneae: Salticidae: Maratus) of the Queensland Museum, including six new species",
					"publicationDate": "",
					"journalTitle": "Zootaxa",
					"journalYear": "2016",
					"journalVolume": "4154",
					"journalIssue": "5",
					"pages": "501–525",
					"authorityName": "",
					"authorityYear": "",
					"kingdom": "Animalia",
					"phylum": "Arthropoda",
					"order": "Araneae",
					"family": "Salticidae",
					"genus": "Maratus",
					"species": "chrysomelas",
					"status": "",
					"taxonomicNameLabel": "",
					"rank": "species",
					"context": "The  <b>Maratus</b> chrysomelas  group        (   FIGURES 1 A, B, D, E, G, H)        Otto & Hill (2016a) described the  <b>Maratus</b> chrysomelas  group (  M. chrysomelas  and  M. nigromaculatus  ) as having a wide fringe at the sides of the opisthosoma and similar courtship displays. We find also this group contains species which have an",
					"_links": {
						"self": {
							"href": "https://zenodeo.punkish.org/treatments?treatmentId=undefined"
						}
					}
				}
			],
			"nextid": 275718,
			"from": 1,
			"to": 30,
			"previd": 0,
			"prevpage": 0,
			"nextpage": 2,
			"facets": {
				"journalVolume": [
					{
						"journalVolume": "112",
						"c": 7
					},
					{
						"journalVolume": "141",
						"c": 8
					},
					{
						"journalVolume": "4000",
						"c": 1
					},
					{
						"journalVolume": "4154",
						"c": 20
					},
					{
						"journalVolume": "4564",
						"c": 4
					}
				],
				"journalTitle": [
					{
						"journalTitle": "Peckhamia",
						"c": 15
					},
					{
						"journalTitle": "Zootaxa",
						"c": 25
					}
				],
				"journalYear": [
					{
						"journalYear": "2014",
						"c": 7
					},
					{
						"journalYear": "2015",
						"c": 1
					},
					{
						"journalYear": "2016",
						"c": 28
					},
					{
						"journalYear": "2019",
						"c": 4
					}
				],
				"kingdom": [
					{
						"kingdom": "Animalia",
						"c": 39
					}
				],
				"phylum": [
					{
						"phylum": "Arthropoda",
						"c": 39
					}
				],
				"order": [
					{
						"order": "Araneae",
						"c": 39
					}
				],
				"family": [
					{
						"family": "Salticidae",
						"c": 39
					}
				],
				"genus": [
					{
						"genus": "Maratus",
						"c": 38
					},
					{
						"genus": "Tauala",
						"c": 1
					}
				],
				"status": [
					{
						"status": "new specIes",
						"c": 1
					},
					{
						"status": "new species",
						"c": 7
					},
					{
						"status": "sp. nov.",
						"c": 10
					}
				],
				"rank": [
					{
						"rank": "genus",
						"c": 5
					},
					{
						"rank": "species",
						"c": 33
					},
					{
						"rank": "variety",
						"c": 1
					}
				],
				"species": [
					{
						"species": "albus",
						"c": 1
					},
					{
						"species": "anomalus",
						"c": 2
					},
					{
						"species": "aquilus",
						"c": 1
					},
					{
						"species": "australis",
						"c": 1
					},
					{
						"species": "avibus",
						"c": 1
					},
					{
						"species": "bubo",
						"c": 1
					},
					{
						"species": "chrysomelas",
						"c": 2
					},
					{
						"species": "combustus",
						"c": 1
					},
					{
						"species": "digitatus",
						"c": 2
					},
					{
						"species": "eliasi",
						"c": 1
					},
					{
						"species": "felinus",
						"c": 1
					},
					{
						"species": "fimbriatus",
						"c": 1
					},
					{
						"species": "julianneae",
						"c": 1
					},
					{
						"species": "karrie",
						"c": 1
					},
					{
						"species": "kiwirrkurra",
						"c": 1
					},
					{
						"species": "licunxini",
						"c": 1
					},
					{
						"species": "lobatus",
						"c": 1
					},
					{
						"species": "melindae",
						"c": 1
					},
					{
						"species": "michaelorum",
						"c": 1
					},
					{
						"species": "mungaich",
						"c": 1
					},
					{
						"species": "ottoi",
						"c": 2
					},
					{
						"species": "pavonis",
						"c": 2
					},
					{
						"species": "sarahae",
						"c": 1
					},
					{
						"species": "speciosus",
						"c": 1
					},
					{
						"species": "tessellatus",
						"c": 1
					},
					{
						"species": "vespa",
						"c": 1
					},
					{
						"species": "volans",
						"c": 2
					},
					{
						"species": "vultus",
						"c": 1
					}
				],
				"collectionCode": [
					{
						"collectionCode": "MALE",
						"c": 17
					},
					{
						"collectionCode": "NSW",
						"c": 2
					},
					{
						"collectionCode": "Western Australian Museum, Perth",
						"c": 1
					}
				]
			},
			"stats": {
				"specimens": [
					{
						"Sum(specimenCount)": 78
					}
				],
				"male specimens": [
					{
						"Sum(specimenCountMale)": null
					}
				],
				"female specimens": [
					{
						"Sum(specimenCountFemale)": null
					}
				],
				"treatments with specimens": [
					{
						"Count(DISTINCT treatments.treatmentId)": 20
					}
				],
				"treatments with male specimens": [
					{
						"Count(DISTINCT treatments.treatmentId)": 0
					}
				],
				"treatments with female specimens": [
					{
						"Count(DISTINCT treatments.treatmentId)": 0
					}
				],
				"figure citations": [
					{
						"Count(figureCitationId)": 301
					}
				]
			}
		},
		"stored": 1582637492962,
		"ttl": 86367574,
		"isStale": false
	},
	"report": {
		"msec": 1.3718090057373047,
		"stored": 1582637492962,
		"ttl": 86367574,
		"isStale": false
	}
}
```
