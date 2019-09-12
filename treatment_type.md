# Treatment Object Type

* [Fields](#fields)
 * [Zenodeo API treatments parameters](#zenodeo-api-treatments-parameters)
 * [Zenodeo response fields](#zenodeo-response-fields)
* [Sample Zenodeo API response (treatmentID)](#sample-zenodeo-api-response-treatmentid)

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
| pages |  no | no | yes | |
| doi |  no | no | yes | |
| zenodoDep | no | no | no | |
| publicationDate |  no | no | no | |
| *articleTitle* |  no |  no | yes | needed |
| *articleDoi* | no | no | yes | needed |
| journalTitle | yes | no  yes | | 
| journalYear |  yes | yes | yes | | 
| journalVolume |  yes | no | yes | | 
| journalIssue | no | no | yes | |  
| authorityName |  no | no | yes? | | 
| authorityYear |  no | no |yes? | | 
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

## Sample Zenodeo API response (treatmentID)

```
{
  "value": {
    "treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D",
    "treatmentTitle": "Maratus felinus Schubert, 2019, sp. nov.",
    "pages": "81–100",
    "doi": "https://doi.org/10.11646/zootaxa.4564.1.3",
    "zenodoDep": "2588669",
    "publicationDate": "2019-03-05",
    "journalTitle": "Zootaxa",
    "journalYear": "2019",
    "journalVolume": "4564",
    "journalIssue": "1",
    "authorityName": "Schubert",
    "authorityYear": "2019",
    "kingdom": "Animalia",
    "phylum": "Arthropoda",
    "order": "Araneae",
    "family": "Salticidae",
    "genus": "Maratus",
    "species": "felinus",
    "status": "sp. nov.",
    "rank": "species",
    "fullText": "Maratus felinus  sp. nov.       ( FIGURES 2C , 17 A–F, 18A–D, 19A–C, 20A–F, 21A–D, 22A–B, 23A–B)     Material examined.  MALE HOLOTYPE (WAM–T147353) from Australia , Western Australia Lake Jasper , 34°22'42.5\"S , 115°39'27.9\"E ,  48m  , M. Duncan ,  25 Sep. 2018   .  PARATYPES : 1 male , 2 female (WAM-T147354), same collection data as holotype  .     Etymology. The specific name (  felinus , Latin  , m., adjective, English translation: feline) refers to the markings on the dorsal opisthosomal plate which resemble a cat.     FIGURE 17. Habitus images of living holotype  Maratus felinus   sp. nov.  (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.     FIGURE 18. Habitus images of preserved holotype  Maratus felinus   sp. nov.  (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.     Diagnosis. The male of this species bears some resemblance to  Maratus linnaei  ( Otto & Hill, 2017B ) by the colour of scales covering the ocular quadrangle area and the dark setae below the AME, however, the males lack the heavy cover of long, bristle like setae on legs III.  Maratus felinus  can be distinguished from other  Maratus  species by its atypical ovoid-shaped opisthosoma and by the scale patterns on the dorsal opisthosomal plate. Females of  M. felinus  are similar to other Southwestern Australian endemics such as  M. flavus  ( Otto and Hill 2017A ) and identification is problematic without association with a male. The structures of the external male and female genitalia of  M. felinus  are of no use in distinguishing them from other Southwestern Australia endemic  Maratus  species.     Description. Male (WAM–T147353). Carapace mostly black and glabrous; median thoracic tract comprised of white scales extends from rear slope of carapace to between the PLE; carapace rimmed with well-defined marginal band comprised of white scales ( Figure 17B ); ocular quadrangle region with dense cover of grey scales interrupted by distinct stripes of red scales behind each anterior eye, and at the median ( Figure 17A ).    FIGURE 19. Images of preserved holotype  Maratus felinus   sp. nov.  pedipalp structure (WAM–T147353): A, retrolateral view; B, ventral view showing embolic disc and tegular lobe. C, prolateral view showing finger-like retrolateral tibial apophysis and retrolateral sperm duct loop.     FIGURE 20. Habitus images of living paratype #1 female  Maratus felinus   sp. nov.  (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.    PME closer to PLE than to ALE; AME bordered with dark grey to black scales below, white scales laterally, and dark red scales dorsally; long white setae project downwards from below anterior median eyes above black clypeus; clypeus mostly glabrous besides white setae at median; chelicerae dark brown to black and glabrous ( Figure 18C ); coxae and labium light brown and glabrous; endites dark brown with pale upper edges and glabrous; sternum dark brown ( Figure 18B ) with light covering of fine, white setae.   Opisthosoma distinctively patterned and ovoid in shape; dorsal opisthosomal plate thickly covered with mostly grey-blue/tan scales, edged with dark red and black scales; arcs of white scales bordered by blue scales run parallel to each lateral edge of opisthosoma, extending from white triangular patch of scales at upper margin of opisthosoma; below, two converging lines of white scales bordered by blue extend from each lateral edge of opisthosoma; two diagonal, parallel stripes of white scales bordered by blue scales extend from each posterolateral edge of dorsal opisthosoma; these stripes interrupted by arrow-shaped patch of iridescent blue scales inset with a small black circle of scales extending from posteromedial margin of dorsal opisthosoma to approximately 1/4 the length of opisthosoma ( Figure 17B ).    FIGURE 21. Habitus and epigyne images of preserved paratype #1 female  Maratus felinus   sp. nov.  (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.    Posterior edge of dorsal opisthosomal plate cleaved, extending over opisthosoma when viewed ventrally ( Figure 18B ); long white tufts of setae project from each posterolateral edge of dorsal opisthosomal plate ( Figure 2C ); colular tuft of white setae above black spinnerets; ventral opisthosoma dark grey and scattered with short, creamy coloured setae; minute dorsal opisthosomal flaps fold around opisthosoma, visible when viewed ventrally ( Figure 18B ).   Legs I and II subequal in length; legs III and IV longer; legs III by far longest. Legs IV ringed with alternating bands of dark brown and white setae; femora of legs I and II dorsally and posteriorly marked with dark bands; legs I and II otherwise with light cover of white setae; dorsal surface of legs III dark brown to black; anterior surface of legs III striped with deep red/black markings ( Figure 2C ); ventral surface of femora of legs III striped with white setae; tibiae, metatarsi, and tarsi of legs III fringed with long black and white setae; tarsi of each leg tipped with grey to black setae ( Figure 17 A–F).   Pedipalp covered dorsally with long white setae; relatively large palpal bulb with retrolateral sperm duct loop, large retrobasal tegular lobe, finger-like retrolateral tibial apophysis, embolus with pointed inner apex beneath thicker outer apex ( Figure 19 A–C).   Female (WAM-T147354). Ocular quadrangle with thick cover of red-brown to off-white setae; setation of ocular quadrangle interrupted by glabrous stripes behind each AME exposing dark integument of carapace ( Figure 20 B–F); distinct median thoracic tract of white scales extends from rear slope of carapace to posterior margin of carapace; less distinct bands of white setae extend from below PLE to rear margin of carapace; carapace otherwise dark brown to black and mostly glabrous and lacking marginal band ( Figure 20 B–F).    FIGURE 22. Variation in preserved holotype and paratype male  Maratus felinus   sp. nov.  specimens: A, holotype male; B, paratype male #1.    Anterior eyes bordered with red-brown and white scales dorsally, and white scales laterally and below; PME closer to PLE than to ALE; long white setae project downwards from below AME forming triangular shape; clypeus covered with short, white setae ( Figure 20A ); chelicerae dark brown and glabrous; coxae, endites, and labium dark brown, translucent and mostly glabrous; sternum dark brown with light covering of fine, white setae ( Figure 21A ).   Dorsal opisthosoma dark brown with incomplete cover of off-white and dark brown setae; central spot of offwhite setae on dorsal opisthosoma; surface above each of the four dorsal opisthosomal apodemes glabrous; posterior and lateral edges of dorsal opisthosoma bordered by irregular broad band of off-white and light brown setae; colular tuft of white setae situated above spinnerets ( Figure 20B ); posterior spinnerets dark brown to black, anterior spinnerets lighter brown ( Figure 21B ); lateral and ventral opisthosoma light brown with irregular dark spots ( Figure 21A ).   Legs I and II subequal in length; legs III and IV longer; legs III longest; integument of legs III and IV with alternating bands of black and brown; legs I and II similarly banded but less distinctively so; ventral femoral surface of each leg distinctively marked with dark bands ( Figure 21A ); each leg with light cover of white setae; tarsi of each leg tipped with black setae; pedipalps light brown and translucent with incomplete cover of off-white setae ( Figure 20A ).   Epigynum with pair of large ovate fossae separated by septum; ovate posterior spermatheca behind each fossa; sclerotized ducts present anterior to each spermatheca ( Figure 21D ).   Variation. Patterns may be more distinct or indistinct in both male and female specimens and colours may slightly vary ( Figure 22A and B , 23A and B ).   Dimensions. Male. Total length: 3.77–3.80 (3.79±0.01, n=2). Carapace length 1.72–1.74 (1.73±0.01, n=2). Opisthosoma length 2.05–2.06 (2.06± 0.01, n=2). Leg I length: 2.23–2.85 (2.84±0.01, n=2).  Leg II length: 2.82–2.85 (2.84±0.02, n=2). Leg III length: 4.14–4.20 (4.17±0.03, n=2). Leg IV length: 3.73– 3.76 (3.75±0.02).   FIGURE 23. Variation in preserved paratype male  Maratus felinus   sp. nov.  specimen s: A, paratype female #1; B, paratype female #2.    Dimensions. Female. Total length: 4.95–4.99 (4.97±0.02, n=2). Carapace length 1.88–1.89 (1.89±0.01, n=2). Opisthosoma length 2.00–2.22 (2.11± 0.11, n=2). Leg I length: 2.67–2.70 (2.69±0.02, n=2). Leg II length: 2.66–2.70 (2.68±0.02, n=2). Leg III length: 4.46–4.50 (4.48±0.02, n=2). Leg IV length: 3.88–3.89 (3.88±0.01, n=2).     Distribution. Known only from near Lake Jasper, Western Australia .   Courtship display. The opisthosoma of the male is first elevated and waved. Following this, a single leg III is elevated and waved. The pedipalps are held apart, exposing the chelicerae. The second leg III is elevated and both legs III are held in place while the opisthosoma is intermittently lowered and raised, making slight waving motions as it does so. The female begins approaching the male, and ‘kicking’ motions are made with each leg I, alternating between each leg unpredictably while the opisthosoma is in the lowered position. Legs III become flexed inwards, forming an arc which borders the opisthosoma while it is elevated. (Note: only partial courtship display observed, the males may exhibit more modes of courtship).",
    "search-criteria": {
      "page": "1",
      "size": "30",
      "treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D"
    },
    "_links": {
      "self": {
        "href": "https://zenodeo.punkish.org/v2/treatments?page=1&size=30&treatmentId=03FE87F49704FF86FF15FCE7FD79BC2D"
      }
    },
    "xml": "<document ID-DOI=\"https://doi.org/10.11646/zootaxa.4564.1.3\" ID-ISSN=\"1175-5326\" ID-Zenodo-Dep=\"2588669\" ID-ZooBank=\"B8991FC7-399B-4B00-B968-D3BC44F32020\" _generate=\"added\" checkinTime=\"1552167099920\" checkinUser=\"plazi\" docAuthor=\"Schubert, Joseph\" docDate=\"2019\" docId=\"03FE87F49704FF86FF15FCE7FD79BC2D\" docLanguage=\"en\" docName=\"zootaxa.4564.1.3.pdf\" docOrigin=\"Zootaxa 4564 (1)\" docStyle=\"DocumentStylede.uka.ipd.idaho.easyIO.settings.Settings@107e5441\" docStyleName=\"zootaxa.2013.journal_article\" docTitle=\"Maratus felinus Schubert, 2019, sp. nov.\" docType=\"treatment\" lastPageId=\"19\" lastPageNumber=\"99\" masterDocId=\"FFC7FF8C9709FF95FF82FFBBFFC4BD30\" masterDocTitle=\"Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)\" masterLastPageNumber=\"100\" masterPageNumber=\"81\" pageId=\"13\" pageNumber=\"94\" updateTime=\"1553735656812\" updateUser=\"ImsDioSync\">\n<mods:mods xmlns:mods=\"http://www.loc.gov/mods/v3\">\n<mods:titleInfo>\n<mods:title>Three new peacock spiders from Southwestern Australia (Araneae: Salticidae: Euophryini: Maratus Karsch, 1878)</mods:title>\n</mods:titleInfo>\n<mods:name type=\"personal\">\n<mods:role>\n<mods:roleTerm>Author</mods:roleTerm>\n</mods:role>\n<mods:namePart>Schubert, Joseph</mods:namePart>\n</mods:name>\n<mods:typeOfResource>text</mods:typeOfResource>\n<mods:relatedItem type=\"host\">\n<mods:titleInfo>\n<mods:title>Zootaxa</mods:title>\n</mods:titleInfo>\n<mods:part>\n<mods:date>2019</mods:date>\n<mods:detail type=\"pubDate\">\n<mods:number>2019-03-05</mods:number>\n</mods:detail>\n<mods:detail type=\"volume\">\n<mods:number>4564</mods:number>\n</mods:detail>\n<mods:detail type=\"issue\">\n<mods:number>1</mods:number>\n</mods:detail>\n<mods:extent unit=\"page\">\n<mods:start>81</mods:start>\n<mods:end>100</mods:end>\n</mods:extent>\n</mods:part>\n</mods:relatedItem>\n<mods:classification>journal article</mods:classification>\n<mods:identifier type=\"DOI\">https://doi.org/10.11646/zootaxa.4564.1.3</mods:identifier>\n<mods:identifier type=\"ISSN\">1175-5326</mods:identifier>\n<mods:identifier type=\"Zenodo-Dep\">2588669</mods:identifier>\n<mods:identifier type=\"ZooBank\">B8991FC7-399B-4B00-B968-D3BC44F32020</mods:identifier>\n</mods:mods>\n<treatment LSID=\"urn:lsid:plazi:treatment:03FE87F49704FF86FF15FCE7FD79BC2D\" httpUri=\"http://treatment.plazi.org/id/03FE87F49704FF86FF15FCE7FD79BC2D\" lastPageId=\"19\" lastPageNumber=\"100\" pageId=\"13\" pageNumber=\"94\">\n<subSubSection box=\"[151,445,860,887]\" pageId=\"13\" pageNumber=\"94\" type=\"nomenclature\">\n<paragraph blockId=\"13.[151,983,860,920]\" box=\"[151,445,860,887]\" pageId=\"13\" pageNumber=\"94\">\n<emphasis bold=\"true\" box=\"[151,445,860,887]\" pageId=\"13\" pageNumber=\"94\">\n<heading bold=\"true\" box=\"[151,445,860,887]\" fontSize=\"11\" level=\"1\" pageId=\"13\" pageNumber=\"94\" reason=\"1\">\n<emphasis bold=\"true\" box=\"[151,344,860,886]\" italics=\"true\" pageId=\"13\" pageNumber=\"94\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[151,344,860,886]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"13\" pageNumber=\"94\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<taxonomicNameLabel box=\"[351,445,861,887]\" pageId=\"13\" pageNumber=\"94\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</heading>\n</emphasis>\n</paragraph>\n</subSubSection>\n<subSubSection box=\"[151,983,896,920]\" pageId=\"13\" pageNumber=\"94\" type=\"description\">\n<paragraph blockId=\"13.[151,983,860,920]\" box=\"[151,983,896,920]\" pageId=\"13\" pageNumber=\"94\">\n(\n<figureCitation box=\"[158,319,896,920]\" captionStart=\"FIGURE 2\" captionStartId=\"2.[151,250,645,667]\" captionTargetBox=\"[151,1435,208,604]\" captionTargetId=\"figure@2.[151,1435,208,604]\" captionTargetPageId=\"2\" captionText=\"FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.\" httpUri=\"https://zenodo.org/record/2588673/files/figure.png\" pageId=\"13\" pageNumber=\"94\">FIGURES 2C</figureCitation>\n, \n<figureCitation box=\"[331,356,896,920]\" captionStart=\"FIGURE 17\" captionStartId=\"13.[151,250,1943,1965]\" captionTargetBox=\"[177,1416,1220,1918]\" captionTargetId=\"figure@13.[150,1436,1176,1929]\" captionTargetPageId=\"13\" captionText=\"FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"13\" pageNumber=\"94\">17</figureCitation>\nA–F, 18A–D, 19A–C, 20A–F, 21A–D, 22A–B, 23A–B)\n</paragraph>\n</subSubSection>\n<subSubSection pageId=\"13\" pageNumber=\"94\" type=\"materials_examined\">\n<paragraph blockId=\"13.[151,1436,967,1136]\" pageId=\"13\" pageNumber=\"94\">\n<emphasis bold=\"true\" box=\"[151,391,967,992]\" pageId=\"13\" pageNumber=\"94\">Material examined.</emphasis>\n<materialsCitation collectingDate=\"2018-09-25\" collectionCode=\"MALE\" collectorName=\"M. Duncan\" country=\"Australia\" elevation=\"48\" latitude=\"-34.37847\" location=\"Lake Jasper\" longLatPrecision=\"1\" longitude=\"115.65775\" pageId=\"13\" pageNumber=\"94\" specimenCount=\"1\" stateProvince=\"Western Australia\" typeStatus=\"holotype\">\n<collectionCode box=\"[405,484,968,992]\" pageId=\"13\" pageNumber=\"94\">MALE</collectionCode>\n<typeStatus box=\"[498,646,968,992]\" pageId=\"13\" pageNumber=\"94\">HOLOTYPE</typeStatus>\n(WAM–T147353) from \n<collectingCountry box=\"[945,1051,967,992]\" name=\"Australia\" pageId=\"13\" pageNumber=\"94\">Australia</collectingCountry>\n, \n<collectingRegion box=\"[1069,1276,967,992]\" country=\"Australia\" name=\"Western Australia\" pageId=\"13\" pageNumber=\"94\">Western Australia</collectingRegion>\n<location LSID=\"urn:lsid:plazi:treatment:03FE87F49704FF86FF15FCE7FD79BC2D:8E8860399704FF98FA88FC7CFA5CBEEF\" box=\"[1290,1432,967,992]\" country=\"Australia\" latitude=\"-34.37847\" longLatPrecision=\"1\" longitude=\"115.65775\" name=\"Lake Jasper\" pageId=\"13\" pageNumber=\"94\" stateProvince=\"Western Australia\">Lake Jasper</location>\n, \n<geoCoordinate box=\"[151,302,1004,1029]\" direction=\"south\" orientation=\"latitude\" pageId=\"13\" pageNumber=\"94\" precision=\"1\" value=\"-34.37847\">34°22'42.5&quot;S</geoCoordinate>\n, \n<geoCoordinate box=\"[314,480,1004,1029]\" direction=\"east\" orientation=\"longitude\" pageId=\"13\" pageNumber=\"94\" precision=\"1\" value=\"115.65775\">115°39'27.9&quot;E</geoCoordinate>\n, \n<quantity box=\"[492,545,1004,1028]\" metricMagnitude=\"1\" metricUnit=\"m\" metricValue=\"4.8\" pageId=\"13\" pageNumber=\"94\" unit=\"m\" value=\"48.0\">\n<elevation box=\"[492,545,1004,1028]\" metricMagnitude=\"1\" metricUnit=\"m\" metricValue=\"4.8\" pageId=\"13\" pageNumber=\"94\" unit=\"m\" value=\"48.0\">48m</elevation>\n</quantity>\n, \n<collectorName box=\"[557,687,1005,1028]\" pageId=\"13\" pageNumber=\"94\">M. Duncan</collectorName>\n, \n<date box=\"[699,852,1004,1029]\" pageId=\"13\" pageNumber=\"94\" value=\"2018-09-25\">\n<collectingDate box=\"[699,852,1004,1029]\" pageId=\"13\" pageNumber=\"94\" value=\"2018-09-25\">25 Sep. 2018</collectingDate>\n</date>\n</materialsCitation>\n. \n<materialsCitation collectingDate=\"2018-09-25\" collectionCode=\"MALE\" collectorName=\"M. Duncan\" country=\"Australia\" elevation=\"48\" latitude=\"-34.37847\" location=\"Lake Jasper\" longLatPrecision=\"1\" longitude=\"115.65775\" pageId=\"13\" pageNumber=\"94\" specimenCount=\"3\" specimenCount-female=\"2\" specimenCount-male=\"1\" stateProvince=\"Western Australia\" typeStatus=\"paratype\">\n<typeStatus box=\"[863,1022,1004,1028]\" pageId=\"13\" pageNumber=\"94\">PARATYPES</typeStatus>\n: \n<specimenCount box=\"[1034,1113,1004,1029]\" pageId=\"13\" pageNumber=\"94\" type=\"male\">1 male</specimenCount>\n, \n<specimenCount box=\"[1125,1223,1004,1029]\" pageId=\"13\" pageNumber=\"94\" type=\"female\">2 female</specimenCount>\n(WAM-T147354), same collection data as holotype\n</materialsCitation>\n.\n</paragraph>\n</subSubSection>\n<subSubSection pageId=\"13\" pageNumber=\"94\" type=\"etymology\">\n<paragraph blockId=\"13.[151,1436,967,1136]\" pageId=\"13\" pageNumber=\"94\">\n<emphasis bold=\"true\" box=\"[199,334,1076,1101]\" pageId=\"13\" pageNumber=\"94\">Etymology.</emphasis>\nThe specific name (\n<taxonomicName authority=\", Latin\" authorityName=\"Latin\" box=\"[563,714,1076,1101]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"13\" pageNumber=\"94\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\">\n<emphasis box=\"[563,638,1076,1100]\" italics=\"true\" pageId=\"13\" pageNumber=\"94\">felinus</emphasis>\n, Latin\n</taxonomicName>\n, m., adjective, English translation: feline) refers to the markings on the dorsal opisthosomal plate which resemble a cat.\n</paragraph>\n</subSubSection>\n<paragraph blockId=\"13.[151,1436,1943,1996]\" pageId=\"13\" pageNumber=\"94\">\n<caption httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"13\" pageNumber=\"94\" startId=\"13.[151,250,1943,1965]\" targetBox=\"[177,1416,1220,1918]\" targetPageId=\"13\">\n<emphasis bold=\"true\" box=\"[151,288,1943,1965]\" pageId=\"13\" pageNumber=\"94\">FIGURE 17.</emphasis>\nHabitus images of living holotype \n<emphasis box=\"[648,809,1944,1965]\" italics=\"true\" pageId=\"13\" pageNumber=\"94\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[648,809,1944,1965]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"13\" pageNumber=\"94\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[815,896,1944,1965]\" pageId=\"13\" pageNumber=\"94\">\n<taxonomicNameLabel box=\"[815,896,1944,1965]\" pageId=\"13\" pageNumber=\"94\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\n(WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\n</caption>\n</paragraph>\n<paragraph blockId=\"14.[151,1435,1637,1690]\" pageId=\"14\" pageNumber=\"95\">\n<caption httpUri=\"https://zenodo.org/record/2588707/files/figure.png\" pageId=\"14\" pageNumber=\"95\" startId=\"14.[151,250,1637,1659]\" targetBox=\"[152,1409,210,1598]\" targetPageId=\"14\">\n<emphasis bold=\"true\" box=\"[151,290,1637,1659]\" pageId=\"14\" pageNumber=\"95\">FIGURE 18.</emphasis>\nHabitus images of preserved holotype \n<emphasis box=\"[701,864,1637,1659]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[701,864,1637,1659]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[872,955,1638,1659]\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicNameLabel box=\"[872,955,1638,1659]\" pageId=\"14\" pageNumber=\"95\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\n(WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.\n</caption>\n</paragraph>\n<subSubSection pageId=\"14\" pageNumber=\"95\" type=\"diagnosis\">\n<paragraph blockId=\"14.[151,1437,1734,2011]\" pageId=\"14\" pageNumber=\"95\">\n<emphasis bold=\"true\" box=\"[199,321,1734,1759]\" pageId=\"14\" pageNumber=\"95\">Diagnosis.</emphasis>\nThe male of this species bears some resemblance to \n<emphasis box=\"[927,1107,1734,1758]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Waldock\" authorityYear=\"2008\" box=\"[927,1107,1734,1758]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"linnaei\">Maratus linnaei</taxonomicName>\n</emphasis>\n(\n<bibRefCitation author=\"Otto, J. C. &amp; Hill, D. E.\" box=\"[1124,1349,1734,1759]\" pageId=\"14\" pageNumber=\"95\" pagination=\"1 - 23\" refId=\"ref6047\" refString=\"Otto, J. C. &amp; Hill, D. E. (2017 B) Catalogue of the Australian peacock spiders (Araneae: Salticidae: Euophryini: Maratus, Saratus), version 2. Peckhamia 148 (2), 1 - 23.\" type=\"journal article\" year=\"2017\">Otto &amp; Hill, 2017B</bibRefCitation>\n) by the colour of scales covering the ocular quadrangle area and the dark setae below the AME, however, the males lack the heavy cover of long, bristle like setae on legs III. \n<emphasis box=\"[777,957,1806,1830]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[777,957,1806,1830]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\">Maratus felinus</taxonomicName>\n</emphasis>\ncan be distinguished from other \n<emphasis box=\"[1341,1436,1807,1830]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Karsch\" authorityYear=\"1878\" box=\"[1341,1436,1807,1830]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"genus\">Maratus</taxonomicName>\n</emphasis>\nspecies by its atypical ovoid-shaped opisthosoma and by the scale patterns on the dorsal opisthosomal plate. Females of \n<emphasis box=\"[289,405,1878,1902]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[289,405,1878,1902]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\">M. felinus</taxonomicName>\n</emphasis>\nare similar to other Southwestern Australian endemics such as \n<emphasis box=\"[1153,1261,1878,1902]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Otto &amp; Hill\" authorityYear=\"2018\" box=\"[1153,1261,1878,1902]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"flavus\">M. flavus</taxonomicName>\n</emphasis>\n(\n<bibRefCitation author=\"Otto, J. C. &amp; Hill, D. E.\" pageId=\"14\" pageNumber=\"95\" pagination=\"1 - 23\" refId=\"ref6047\" refString=\"Otto, J. C. &amp; Hill, D. E. (2017 B) Catalogue of the Australian peacock spiders (Araneae: Salticidae: Euophryini: Maratus, Saratus), version 2. Peckhamia 148 (2), 1 - 23.\" type=\"journal article\" year=\"2017\">Otto and Hill 2017A</bibRefCitation>\n) and identification is problematic without association with a male. The structures of the external male and female genitalia of \n<emphasis box=\"[377,493,1950,1974]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[377,493,1950,1974]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\">M. felinus</taxonomicName>\n</emphasis>\nare of no use in distinguishing them from other Southwestern \n<collectingCountry box=\"[1228,1331,1950,1975]\" name=\"Australia\" pageId=\"14\" pageNumber=\"95\">Australia</collectingCountry>\nendemic \n<emphasis box=\"[151,246,1987,2010]\" italics=\"true\" pageId=\"14\" pageNumber=\"95\">\n<taxonomicName authorityName=\"Karsch\" authorityYear=\"1878\" box=\"[151,246,1987,2010]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"14\" pageNumber=\"95\" phylum=\"Arthropoda\" rank=\"genus\">Maratus</taxonomicName>\n</emphasis>\nspecies.\n</paragraph>\n</subSubSection>\n<subSubSection lastPageId=\"18\" lastPageNumber=\"99\" pageId=\"15\" pageNumber=\"96\" type=\"description\">\n<paragraph blockId=\"15.[151,1436,151,285]\" pageId=\"15\" pageNumber=\"96\">\n<emphasis bold=\"true\" box=\"[199,414,151,176]\" pageId=\"15\" pageNumber=\"96\">Description. Male</emphasis>\n(WAM–T147353). Carapace mostly black and glabrous; median thoracic tract comprised of white scales extends from rear slope of carapace to between the PLE; carapace rimmed with well-defined marginal band comprised of white scales (\n<figureCitation box=\"[632,764,223,248]\" captionStart=\"FIGURE 17\" captionStartId=\"13.[151,250,1943,1965]\" captionTargetBox=\"[177,1416,1220,1918]\" captionTargetId=\"figure@13.[150,1436,1176,1929]\" captionTargetPageId=\"13\" captionText=\"FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"15\" pageNumber=\"96\">Figure 17B</figureCitation>\n); ocular quadrangle region with dense cover of grey scales interrupted by distinct stripes of red scales behind each anterior eye, and at the median (\n<figureCitation box=\"[1133,1268,260,285]\" captionStart=\"FIGURE 17\" captionStartId=\"13.[151,250,1943,1965]\" captionTargetBox=\"[177,1416,1220,1918]\" captionTargetId=\"figure@13.[150,1436,1176,1929]\" captionTargetPageId=\"13\" captionText=\"FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"15\" pageNumber=\"96\">Figure 17A</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"15.[151,1436,995,1078]\" pageId=\"15\" pageNumber=\"96\">\n<caption httpUri=\"https://zenodo.org/record/2588709/files/figure.png\" pageId=\"15\" pageNumber=\"96\" startId=\"15.[151,250,995,1017]\" targetBox=\"[179,1360,364,928]\" targetPageId=\"15\">\n<emphasis bold=\"true\" box=\"[151,287,995,1017]\" pageId=\"15\" pageNumber=\"96\">FIGURE 19.</emphasis>\nImages of preserved holotype \n<emphasis box=\"[597,757,995,1017]\" italics=\"true\" pageId=\"15\" pageNumber=\"96\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[597,757,995,1017]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"15\" pageNumber=\"96\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[762,841,995,1016]\" pageId=\"15\" pageNumber=\"96\">\n<taxonomicNameLabel box=\"[762,841,995,1016]\" pageId=\"15\" pageNumber=\"96\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\npedipalp structure (WAM–T147353): A, retrolateral view; B, ventral view showing embolic disc and tegular lobe. C, prolateral view showing finger-like retrolateral tibial apophysis and retrolateral sperm duct loop.\n</caption>\n</paragraph>\n<paragraph blockId=\"15.[151,1435,1959,2011]\" pageId=\"15\" pageNumber=\"96\">\n<caption httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"15\" pageNumber=\"96\" startId=\"15.[151,250,1959,1981]\" targetBox=\"[164,1417,1154,1916]\" targetPageId=\"15\">\n<emphasis bold=\"true\" box=\"[151,290,1959,1981]\" pageId=\"15\" pageNumber=\"96\">FIGURE 20.</emphasis>\nHabitus images of living paratype #1 female \n<emphasis box=\"[770,932,1959,1981]\" italics=\"true\" pageId=\"15\" pageNumber=\"96\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[770,932,1959,1981]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"15\" pageNumber=\"96\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[940,1023,1959,1980]\" pageId=\"15\" pageNumber=\"96\">\n<taxonomicNameLabel box=\"[940,1023,1959,1980]\" pageId=\"15\" pageNumber=\"96\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\n(WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\n</caption>\n</paragraph>\n<paragraph blockId=\"16.[151,1437,151,608]\" pageId=\"16\" pageNumber=\"97\">\nPME closer to PLE than to ALE; AME bordered with dark grey to black scales below, white scales laterally, and dark red scales dorsally; long white setae project downwards from below anterior median eyes above black clypeus; clypeus mostly glabrous besides white setae at median; chelicerae dark brown to black and glabrous (\n<figureCitation box=\"[158,290,260,285]\" captionStart=\"FIGURE 18\" captionStartId=\"14.[151,250,1637,1659]\" captionTargetBox=\"[152,1409,210,1598]\" captionTargetId=\"figure@14.[151,1435,193,1616]\" captionTargetPageId=\"14\" captionText=\"FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.\" httpUri=\"https://zenodo.org/record/2588707/files/figure.png\" pageId=\"16\" pageNumber=\"97\">Figure 18C</figureCitation>\n); coxae and labium light brown and glabrous; endites dark brown with pale upper edges and glabrous; sternum dark brown (\n<figureCitation box=\"[391,520,295,320]\" captionStart=\"FIGURE 18\" captionStartId=\"14.[151,250,1637,1659]\" captionTargetBox=\"[152,1409,210,1598]\" captionTargetId=\"figure@14.[151,1435,193,1616]\" captionTargetPageId=\"14\" captionText=\"FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.\" httpUri=\"https://zenodo.org/record/2588707/files/figure.png\" pageId=\"16\" pageNumber=\"97\">Figure 18B</figureCitation>\n) with light covering of fine, white setae.\n</paragraph>\n<paragraph blockId=\"16.[151,1437,151,608]\" pageId=\"16\" pageNumber=\"97\">\nOpisthosoma distinctively patterned and ovoid in shape; dorsal opisthosomal plate thickly covered with mostly grey-blue/tan scales, edged with dark red and black scales; arcs of white scales bordered by blue scales run parallel to each lateral edge of opisthosoma, extending from white triangular patch of scales at upper margin of opisthosoma; below, two converging lines of white scales bordered by blue extend from each lateral edge of opisthosoma; two diagonal, parallel stripes of white scales bordered by blue scales extend from each posterolateral edge of dorsal opisthosoma; these stripes interrupted by arrow-shaped patch of iridescent blue scales inset with a small black circle of scales extending from posteromedial margin of dorsal opisthosoma to approximately 1/4 the length of opisthosoma (\n<figureCitation box=\"[414,546,583,608]\" captionStart=\"FIGURE 17\" captionStartId=\"13.[151,250,1943,1965]\" captionTargetBox=\"[177,1416,1220,1918]\" captionTargetId=\"figure@13.[150,1436,1176,1929]\" captionTargetPageId=\"13\" captionText=\"FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"16\" pageNumber=\"97\">Figure 17B</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"16.[151,1436,1962,2015]\" pageId=\"16\" pageNumber=\"97\">\n<caption httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"16\" pageNumber=\"97\" startId=\"16.[151,250,1962,1984]\" targetBox=\"[150,1436,683,1925]\" targetPageId=\"16\">\n<emphasis bold=\"true\" box=\"[151,290,1962,1984]\" pageId=\"16\" pageNumber=\"97\">FIGURE 21.</emphasis>\nHabitus and epigyne images of preserved paratype #1 female \n<emphasis box=\"[950,1113,1962,1984]\" italics=\"true\" pageId=\"16\" pageNumber=\"97\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[950,1113,1962,1984]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"16\" pageNumber=\"97\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<taxonomicNameLabel box=\"[1122,1205,1962,1983]\" pageId=\"16\" pageNumber=\"97\" rank=\"species\">\n<emphasis bold=\"true\" box=\"[1122,1205,1962,1983]\" pageId=\"16\" pageNumber=\"97\">sp. nov.</emphasis>\n</taxonomicNameLabel>\n(WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\n</caption>\n</paragraph>\n<paragraph blockId=\"17.[151,1437,151,824]\" pageId=\"17\" pageNumber=\"98\">\nPosterior edge of dorsal opisthosomal plate cleaved, extending over opisthosoma when viewed ventrally (\n<figureCitation box=\"[158,291,188,213]\" captionStart=\"FIGURE 18\" captionStartId=\"14.[151,250,1637,1659]\" captionTargetBox=\"[152,1409,210,1598]\" captionTargetId=\"figure@14.[151,1435,193,1616]\" captionTargetPageId=\"14\" captionText=\"FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.\" httpUri=\"https://zenodo.org/record/2588707/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 18B</figureCitation>\n); long white tufts of setae project from each posterolateral edge of dorsal opisthosomal plate (\n<figureCitation captionStart=\"FIGURE 2\" captionStartId=\"2.[151,250,645,667]\" captionTargetBox=\"[151,1435,208,604]\" captionTargetId=\"figure@2.[151,1435,208,604]\" captionTargetPageId=\"2\" captionText=\"FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.\" httpUri=\"https://zenodo.org/record/2588673/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 2C</figureCitation>\n); colular tuft of white setae above black spinnerets; ventral opisthosoma dark grey and scattered with short, creamy coloured setae; minute dorsal opisthosomal flaps fold around opisthosoma, visible when viewed ventrally (\n<figureCitation box=\"[158,290,295,320]\" captionStart=\"FIGURE 18\" captionStartId=\"14.[151,250,1637,1659]\" captionTargetBox=\"[152,1409,210,1598]\" captionTargetId=\"figure@14.[151,1435,193,1616]\" captionTargetPageId=\"14\" captionText=\"FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.\" httpUri=\"https://zenodo.org/record/2588707/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 18B</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"17.[151,1437,151,824]\" pageId=\"17\" pageNumber=\"98\">\nLegs I and II subequal in length; legs III and IV longer; legs III by far longest. Legs IV ringed with alternating bands of dark brown and white setae; femora of legs I and II dorsally and posteriorly marked with dark bands; legs I and II otherwise with light cover of white setae; dorsal surface of legs III dark brown to black; anterior surface of legs III striped with deep red/black markings (\n<figureCitation box=\"[676,795,439,464]\" captionStart=\"FIGURE 2\" captionStartId=\"2.[151,250,645,667]\" captionTargetBox=\"[151,1435,208,604]\" captionTargetId=\"figure@2.[151,1435,208,604]\" captionTargetPageId=\"2\" captionText=\"FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.\" httpUri=\"https://zenodo.org/record/2588673/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 2C</figureCitation>\n); ventral surface of femora of legs III striped with white setae; tibiae, metatarsi, and tarsi of legs III fringed with long black and white setae; tarsi of each leg tipped with grey to black setae (\n<figureCitation box=\"[375,483,511,536]\" captionStart=\"FIGURE 17\" captionStartId=\"13.[151,250,1943,1965]\" captionTargetBox=\"[177,1416,1220,1918]\" captionTargetId=\"figure@13.[150,1436,1176,1929]\" captionTargetPageId=\"13\" captionText=\"FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588705/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 17</figureCitation>\nA–F).\n</paragraph>\n<paragraph blockId=\"17.[151,1437,151,824]\" pageId=\"17\" pageNumber=\"98\">\nPedipalp covered dorsally with long white setae; relatively large palpal bulb with retrolateral sperm duct loop, large retrobasal tegular lobe, finger-like retrolateral tibial apophysis, embolus with pointed inner apex beneath thicker outer apex (\n<figureCitation box=\"[368,476,620,645]\" captionStart=\"FIGURE 19\" captionStartId=\"15.[151,250,995,1017]\" captionTargetBox=\"[179,1360,364,928]\" captionTargetId=\"figure@15.[150,1437,337,974]\" captionTargetPageId=\"15\" captionText=\"FIGURE 19. Images of preserved holotype Maratus felinus sp. nov. pedipalp structure (WAM–T147353): A, retrolateral view; B, ventral view showing embolic disc and tegular lobe. C, prolateral view showing finger-like retrolateral tibial apophysis and retrolateral sperm duct loop.\" httpUri=\"https://zenodo.org/record/2588709/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 19</figureCitation>\nA–C).\n</paragraph>\n<paragraph blockId=\"17.[151,1437,151,824]\" pageId=\"17\" pageNumber=\"98\">\n<emphasis bold=\"true\" box=\"[199,286,655,680]\" pageId=\"17\" pageNumber=\"98\">Female</emphasis>\n(WAM-T147354). Ocular quadrangle with thick cover of red-brown to off-white setae; setation of ocular quadrangle interrupted by glabrous stripes behind each AME exposing dark integument of carapace (\n<figureCitation captionStart=\"FIGURE 20\" captionStartId=\"15.[151,250,1959,1981]\" captionTargetBox=\"[164,1417,1154,1916]\" captionTargetId=\"figure@15.[151,1436,1128,1937]\" captionTargetPageId=\"15\" captionText=\"FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 20</figureCitation>\nB–F); distinct median thoracic tract of white scales extends from rear slope of carapace to posterior margin of carapace; less distinct bands of white setae extend from below PLE to rear margin of carapace; carapace otherwise dark brown to black and mostly glabrous and lacking marginal band (\n<figureCitation box=\"[929,1040,799,824]\" captionStart=\"FIGURE 20\" captionStartId=\"15.[151,250,1959,1981]\" captionTargetBox=\"[164,1417,1154,1916]\" captionTargetId=\"figure@15.[151,1436,1128,1937]\" captionTargetPageId=\"15\" captionText=\"FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 20</figureCitation>\nB–F).\n</paragraph>\n<paragraph blockId=\"17.[151,1435,1690,1742]\" pageId=\"17\" pageNumber=\"98\">\n<caption httpUri=\"https://zenodo.org/record/2588717/files/figure.png\" pageId=\"17\" pageNumber=\"98\" startId=\"17.[151,250,1690,1712]\" targetBox=\"[215,1436,903,1625]\" targetPageId=\"17\">\n<emphasis bold=\"true\" box=\"[151,290,1690,1712]\" pageId=\"17\" pageNumber=\"98\">FIGURE 22.</emphasis>\nVariation in preserved holotype and paratype male \n<emphasis box=\"[832,995,1690,1712]\" italics=\"true\" pageId=\"17\" pageNumber=\"98\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[832,995,1690,1712]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"17\" pageNumber=\"98\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[1003,1086,1690,1711]\" pageId=\"17\" pageNumber=\"98\">\n<taxonomicNameLabel box=\"[1003,1086,1690,1711]\" pageId=\"17\" pageNumber=\"98\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\nspecimens: A, holotype male; B, paratype male #1.\n</caption>\n</paragraph>\n<paragraph blockId=\"17.[151,1436,1781,2022]\" pageId=\"17\" pageNumber=\"98\">\nAnterior eyes bordered with red-brown and white scales dorsally, and white scales laterally and below; PME closer to PLE than to ALE; long white setae project downwards from below AME forming triangular shape; clypeus covered with short, white setae (\n<figureCitation box=\"[625,763,1853,1878]\" captionStart=\"FIGURE 20\" captionStartId=\"15.[151,250,1959,1981]\" captionTargetBox=\"[164,1417,1154,1916]\" captionTargetId=\"figure@15.[151,1436,1128,1937]\" captionTargetPageId=\"15\" captionText=\"FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 20A</figureCitation>\n); chelicerae dark brown and glabrous; coxae, endites, and labium dark brown, translucent and mostly glabrous; sternum dark brown with light covering of fine, white setae (\n<figureCitation box=\"[158,292,1925,1950]\" captionStart=\"FIGURE 21\" captionStartId=\"16.[151,250,1962,1984]\" captionTargetBox=\"[150,1436,683,1925]\" captionTargetId=\"figure@16.[150,1436,683,1925]\" captionTargetPageId=\"16\" captionText=\"FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\" httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"17\" pageNumber=\"98\">Figure 21A</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"17.[151,1436,1781,2022]\" lastBlockId=\"18.[151,1436,151,752]\" lastPageId=\"18\" lastPageNumber=\"99\" pageId=\"17\" pageNumber=\"98\">\nDorsal opisthosoma dark brown with incomplete cover of off-white and dark brown setae; central spot of offwhite setae on dorsal opisthosoma; surface above each of the four dorsal opisthosomal apodemes glabrous; posterior and lateral edges of dorsal opisthosoma bordered by irregular broad band of off-white and light brown setae; colular tuft of white setae situated above spinnerets (\n<figureCitation box=\"[819,952,188,213]\" captionStart=\"FIGURE 20\" captionStartId=\"15.[151,250,1959,1981]\" captionTargetBox=\"[164,1417,1154,1916]\" captionTargetId=\"figure@15.[151,1436,1128,1937]\" captionTargetPageId=\"15\" captionText=\"FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 20B</figureCitation>\n); posterior spinnerets dark brown to black, anterior spinnerets lighter brown (\n<figureCitation box=\"[545,680,223,248]\" captionStart=\"FIGURE 21\" captionStartId=\"16.[151,250,1962,1984]\" captionTargetBox=\"[150,1436,683,1925]\" captionTargetId=\"figure@16.[150,1436,683,1925]\" captionTargetPageId=\"16\" captionText=\"FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\" httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 21B</figureCitation>\n); lateral and ventral opisthosoma light brown with irregular dark spots (\n<figureCitation box=\"[223,357,260,285]\" captionStart=\"FIGURE 21\" captionStartId=\"16.[151,250,1962,1984]\" captionTargetBox=\"[150,1436,683,1925]\" captionTargetId=\"figure@16.[150,1436,683,1925]\" captionTargetPageId=\"16\" captionText=\"FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\" httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 21A</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"18.[151,1436,151,752]\" pageId=\"18\" pageNumber=\"99\">\nLegs I and II subequal in length; legs III and IV longer; legs III longest; integument of legs III and IV with alternating bands of black and brown; legs I and II similarly banded but less distinctively so; ventral femoral surface of each leg distinctively marked with dark bands (\n<figureCitation box=\"[817,952,367,392]\" captionStart=\"FIGURE 21\" captionStartId=\"16.[151,250,1962,1984]\" captionTargetBox=\"[150,1436,683,1925]\" captionTargetId=\"figure@16.[150,1436,683,1925]\" captionTargetPageId=\"16\" captionText=\"FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\" httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 21A</figureCitation>\n); each leg with light cover of white setae; tarsi of each leg tipped with black setae; pedipalps light brown and translucent with incomplete cover of off-white setae (\n<figureCitation box=\"[221,356,439,464]\" captionStart=\"FIGURE 20\" captionStartId=\"15.[151,250,1959,1981]\" captionTargetBox=\"[164,1417,1154,1916]\" captionTargetId=\"figure@15.[151,1436,1128,1937]\" captionTargetPageId=\"15\" captionText=\"FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.\" httpUri=\"https://zenodo.org/record/2588711/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 20A</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"18.[151,1436,151,752]\" pageId=\"18\" pageNumber=\"99\">\nEpigynum with pair of large ovate fossae separated by septum; ovate posterior spermatheca behind each fossa; sclerotized ducts present anterior to each spermatheca (\n<figureCitation box=\"[769,903,511,536]\" captionStart=\"FIGURE 21\" captionStartId=\"16.[151,250,1962,1984]\" captionTargetBox=\"[150,1436,683,1925]\" captionTargetId=\"figure@16.[150,1436,683,1925]\" captionTargetPageId=\"16\" captionText=\"FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.\" httpUri=\"https://zenodo.org/record/2588715/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 21D</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"18.[151,1436,151,752]\" pageId=\"18\" pageNumber=\"99\">\n<emphasis bold=\"true\" box=\"[199,319,548,573]\" pageId=\"18\" pageNumber=\"99\">Variation.</emphasis>\nPatterns may be more distinct or indistinct in both male and female specimens and colours may slightly vary (\n<figureCitation box=\"[306,512,583,608]\" captionStart=\"FIGURE 22\" captionStartId=\"17.[151,250,1690,1712]\" captionTargetBox=\"[215,1436,903,1625]\" captionTargetId=\"figure@17.[150,1436,877,1668]\" captionTargetPageId=\"17\" captionText=\"FIGURE 22. Variation in preserved holotype and paratype male Maratus felinus sp. nov. specimens: A, holotype male; B, paratype male 1.\" httpUri=\"https://zenodo.org/record/2588717/files/figure.png\" pageId=\"18\" pageNumber=\"99\">Figure 22A and B</figureCitation>\n, \n<figureCitation box=\"[523,647,583,608]\" captionStart=\"FIGURE 23\" captionStartId=\"18.[151,250,1646,1668]\" captionTargetBox=\"[176,1391,830,1580]\" captionTargetId=\"figure@18.[151,1436,805,1624]\" captionTargetPageId=\"18\" captionText=\"FIGURE 23. Variation in preserved paratype male Maratus felinus sp. nov. specimens: A, paratype female 1; B, paratype female 2.\" httpUri=\"https://zenodo.org/record/2588719/files/figure.png\" pageId=\"18\" pageNumber=\"99\">23A and B</figureCitation>\n).\n</paragraph>\n<paragraph blockId=\"18.[151,1436,151,752]\" pageId=\"18\" pageNumber=\"99\">\n<emphasis bold=\"true\" box=\"[199,422,620,645]\" pageId=\"18\" pageNumber=\"99\">Dimensions. Male.</emphasis>\nTotal length: 3.77–3.80 (3.79±0.01, n=2). Carapace length 1.72–1.74 (1.73±0.01, n=2). Opisthosoma length 2.05–2.06 (2.06± 0.01, n=2). Leg I length: 2.23–2.85 (2.84±0.01, n=2).\n</paragraph>\n<paragraph blockId=\"18.[151,1436,151,752]\" pageId=\"18\" pageNumber=\"99\">Leg II length: 2.82–2.85 (2.84±0.02, n=2). Leg III length: 4.14–4.20 (4.17±0.03, n=2). Leg IV length: 3.73– 3.76 (3.75±0.02).</paragraph>\n<paragraph blockId=\"18.[151,1436,1646,1698]\" pageId=\"18\" pageNumber=\"99\">\n<caption httpUri=\"https://zenodo.org/record/2588719/files/figure.png\" pageId=\"18\" pageNumber=\"99\" startId=\"18.[151,250,1646,1668]\" targetBox=\"[176,1391,830,1580]\" targetPageId=\"18\">\n<emphasis bold=\"true\" box=\"[151,289,1646,1668]\" pageId=\"18\" pageNumber=\"99\">FIGURE 23.</emphasis>\nVariation in preserved paratype male \n<emphasis box=\"[687,849,1646,1668]\" italics=\"true\" pageId=\"18\" pageNumber=\"99\">\n<taxonomicName authority=\"Schubert, 2019\" authorityName=\"Schubert\" authorityYear=\"2019\" box=\"[687,849,1646,1668]\" class=\"Arachnida\" family=\"Salticidae\" genus=\"Maratus\" higherTaxonomySource=\"GBIF\" kingdom=\"Animalia\" order=\"Araneae\" pageId=\"18\" pageNumber=\"99\" phylum=\"Arthropoda\" rank=\"species\" species=\"felinus\" status=\"sp. nov.\">Maratus felinus</taxonomicName>\n</emphasis>\n<emphasis bold=\"true\" box=\"[857,939,1646,1667]\" pageId=\"18\" pageNumber=\"99\">\n<taxonomicNameLabel box=\"[857,939,1646,1667]\" pageId=\"18\" pageNumber=\"99\" rank=\"species\">sp. nov.</taxonomicNameLabel>\n</emphasis>\nspecimen \n<emphasis bold=\"true\" box=\"[1044,1062,1646,1667]\" pageId=\"18\" pageNumber=\"99\">s:</emphasis>\nA, paratype female #1; B, paratype female #2.\n</caption>\n</paragraph>\n<paragraph blockId=\"18.[151,1437,1743,2020]\" pageId=\"18\" pageNumber=\"99\">\n<emphasis bold=\"true\" box=\"[199,446,1743,1768]\" pageId=\"18\" pageNumber=\"99\">Dimensions. Female.</emphasis>\nTotal length: 4.95–4.99 (4.97±0.02, n=2). Carapace length 1.88–1.89 (1.89±0.01, n=2). Opisthosoma length 2.00–2.22 (2.11± 0.11, n=2). Leg I length: 2.67–2.70 (2.69±0.02, n=2). Leg II length: 2.66–2.70 (2.68±0.02, n=2). Leg III length: 4.46–4.50 (4.48±0.02, n=2). Leg IV length: 3.88–3.89 (3.88±0.01, n=2).\n</paragraph>\n</subSubSection>\n<subSubSection lastPageId=\"19\" lastPageNumber=\"100\" pageId=\"18\" pageNumber=\"99\" type=\"distribution\">\n<paragraph blockId=\"18.[151,1437,1743,2020]\" box=\"[199,976,1887,1912]\" pageId=\"18\" pageNumber=\"99\">\n<emphasis bold=\"true\" box=\"[199,352,1887,1912]\" pageId=\"18\" pageNumber=\"99\">Distribution.</emphasis>\nKnown only from near Lake Jasper, \n<collectingRegion box=\"[768,972,1887,1912]\" country=\"Australia\" name=\"Western Australia\" pageId=\"18\" pageNumber=\"99\">Western Australia</collectingRegion>\n.\n</paragraph>\n<paragraph blockId=\"18.[151,1437,1743,2020]\" lastBlockId=\"19.[151,1437,151,285]\" lastPageId=\"19\" lastPageNumber=\"100\" pageId=\"18\" pageNumber=\"99\">\n<emphasis bold=\"true\" box=\"[199,418,1923,1948]\" pageId=\"18\" pageNumber=\"99\">Courtship display.</emphasis>\nThe opisthosoma of the male is first elevated and waved. Following this, a single leg III is elevated and waved. The pedipalps are held apart, exposing the chelicerae. The second leg III is elevated and both legs III are held in place while the opisthosoma is intermittently lowered and raised, making slight waving motions as it does so. The female begins approaching the male, and ‘kicking’ motions are made with each leg I, alternating between each leg unpredictably while the opisthosoma is in the lowered position. Legs III become flexed inwards, forming an arc which borders the opisthosoma while it is elevated. (Note: only partial courtship display observed, the males may exhibit more modes of courtship).\n</paragraph>\n</subSubSection>\n</treatment>\n</document>",
    "taxonStats": {
      "kingdom": {
        "qryObj": {
          "kingdom": "Animalia"
        },
        "num": {
          "num": 267889
        }
      },
      "phylum": {
        "qryObj": {
          "kingdom": "Animalia",
          "phylum": "Arthropoda"
        },
        "num": {
          "num": 212305
        }
      },
      "order": {
        "qryObj": {
          "kingdom": "Animalia",
          "phylum": "Arthropoda",
          "order": "Araneae"
        },
        "num": {
          "num": 11506
        }
      },
      "family": {
        "qryObj": {
          "kingdom": "Animalia",
          "phylum": "Arthropoda",
          "order": "Araneae",
          "family": "Salticidae"
        },
        "num": {
          "num": 1253
        }
      },
      "genus": {
        "qryObj": {
          "kingdom": "Animalia",
          "phylum": "Arthropoda",
          "order": "Araneae",
          "family": "Salticidae",
          "genus": "Maratus"
        },
        "num": {
          "num": 38
        }
      },
      "species": {
        "qryObj": {
          "kingdom": "Animalia",
          "phylum": "Arthropoda",
          "order": "Araneae",
          "family": "Salticidae",
          "genus": "Maratus",
          "species": "felinus"
        },
        "num": {
          "num": 1
        }
      }
    },
    "related-records": {
      "treatmentAuthors": [
        {
          "treatmentAuthorId": "6cdfe84d-b9af-585c-afaf-ca8172bd5743",
          "author": "Schubert, Joseph",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/treatmentauthors?treatmentAuthorId=6cdfe84d-b9af-585c-afaf-ca8172bd5743"
            }
          }
        }
      ],
      "bibRefCitations": [
        {
          "bibRefCitationId": "1f93485a-f22e-5f45-ba07-cfa99ae9804f",
          "citation": "Otto, J. C. & Hill, D. E. (2017 B) Catalogue of the Australian peacock spiders (Araneae: Salticidae: Euophryini: Maratus, Saratus), version 2. Peckhamia 148 (2), 1 - 23.",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/bibrefcitations?bibRefCitationId=1f93485a-f22e-5f45-ba07-cfa99ae9804f"
            }
          }
        },
        {
          "bibRefCitationId": "23218406-871a-54e4-9f92-6ade8d6cfe1f",
          "citation": "Otto, J. C. & Hill, D. E. (2017 B) Catalogue of the Australian peacock spiders (Araneae: Salticidae: Euophryini: Maratus, Saratus), version 2. Peckhamia 148 (2), 1 - 23.",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/bibrefcitations?bibRefCitationId=23218406-871a-54e4-9f92-6ade8d6cfe1f"
            }
          }
        }
      ],
      "materialsCitations": [
        {
          "materialsCitationId": "7e1637d7-87e8-5c46-a635-a4b61e1b4509",
          "treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D",
          "typeStatus": "holotype",
          "latitude": -34.37847,
          "longitude": 115.65775,
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/materialscitations?materialsCitationId=7e1637d7-87e8-5c46-a635-a4b61e1b4509"
            }
          }
        },
        {
          "materialsCitationId": "ac858ce9-1011-5f27-9a93-0541876a6127",
          "treatmentId": "03FE87F49704FF86FF15FCE7FD79BC2D",
          "typeStatus": "paratype",
          "latitude": -34.37847,
          "longitude": 115.65775,
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/materialscitations?materialsCitationId=ac858ce9-1011-5f27-9a93-0541876a6127"
            }
          }
        }
      ],
      "figureCitations": [
        {
          "figureCitationId": "0795e5da-5464-52d2-a358-1aa8303288ae",
          "captionText": "FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.",
          "httpUri": "https://zenodo.org/record/2588673/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=0795e5da-5464-52d2-a358-1aa8303288ae"
            }
          }
        },
        {
          "figureCitationId": "875f07c8-793f-563e-99db-3a4618038b8f",
          "captionText": "FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588705/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=875f07c8-793f-563e-99db-3a4618038b8f"
            }
          }
        },
        {
          "figureCitationId": "5962dbe9-b005-5b51-af0a-32e1a59215a0",
          "captionText": "FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588705/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=5962dbe9-b005-5b51-af0a-32e1a59215a0"
            }
          }
        },
        {
          "figureCitationId": "8b307c96-e8e5-53c6-9570-7202f6709fe1",
          "captionText": "FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588705/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=8b307c96-e8e5-53c6-9570-7202f6709fe1"
            }
          }
        },
        {
          "figureCitationId": "fd89065c-9173-5093-9891-ec3cad10bd47",
          "captionText": "FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.",
          "httpUri": "https://zenodo.org/record/2588707/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=fd89065c-9173-5093-9891-ec3cad10bd47"
            }
          }
        },
        {
          "figureCitationId": "9cf5950b-730a-5d0a-8288-82db25c9d4da",
          "captionText": "FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.",
          "httpUri": "https://zenodo.org/record/2588707/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=9cf5950b-730a-5d0a-8288-82db25c9d4da"
            }
          }
        },
        {
          "figureCitationId": "9f8844f1-951b-5861-85dc-5480957ab2dd",
          "captionText": "FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588705/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=9f8844f1-951b-5861-85dc-5480957ab2dd"
            }
          }
        },
        {
          "figureCitationId": "7e0e6a40-cfa3-5c68-95e9-3bfd3708611f",
          "captionText": "FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.",
          "httpUri": "https://zenodo.org/record/2588707/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=7e0e6a40-cfa3-5c68-95e9-3bfd3708611f"
            }
          }
        },
        {
          "figureCitationId": "cccaa49f-a87b-531b-ba35-ca80f7159b1b",
          "captionText": "FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.",
          "httpUri": "https://zenodo.org/record/2588673/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=cccaa49f-a87b-531b-ba35-ca80f7159b1b"
            }
          }
        },
        {
          "figureCitationId": "e9261375-260f-51e3-8dac-8ca7d1d62879",
          "captionText": "FIGURE 18. Habitus images of preserved holotype Maratus felinus sp. nov. (WAM–T147353): A, dorsal view; B, ventral view; C, anterior view; D, lateral view.",
          "httpUri": "https://zenodo.org/record/2588707/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=e9261375-260f-51e3-8dac-8ca7d1d62879"
            }
          }
        },
        {
          "figureCitationId": "34799047-a76e-5798-8691-f5bb7ffbaa83",
          "captionText": "FIGURE 2. Living male paratype Maratus aquilus sp. nov., M. combustus sp. nov., and M. felinus sp. nov. performing courtship display to nearby female: A, Courtship display of male Maratus aquilus sp. nov.; B, courtship display of Maratus combustus sp. nov.; C, courtship display of Maratus felinus sp. nov.",
          "httpUri": "https://zenodo.org/record/2588673/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=34799047-a76e-5798-8691-f5bb7ffbaa83"
            }
          }
        },
        {
          "figureCitationId": "354bda7b-20d2-5b31-99cf-8e3442313ac1",
          "captionText": "FIGURE 17. Habitus images of living holotype Maratus felinus sp. nov. (WAM–T147353): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, posterolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588705/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=354bda7b-20d2-5b31-99cf-8e3442313ac1"
            }
          }
        },
        {
          "figureCitationId": "606ea1af-920a-5f55-9658-a568af1c4cbf",
          "captionText": "FIGURE 19. Images of preserved holotype Maratus felinus sp. nov. pedipalp structure (WAM–T147353): A, retrolateral view; B, ventral view showing embolic disc and tegular lobe. C, prolateral view showing finger-like retrolateral tibial apophysis and retrolateral sperm duct loop.",
          "httpUri": "https://zenodo.org/record/2588709/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=606ea1af-920a-5f55-9658-a568af1c4cbf"
            }
          }
        },
        {
          "figureCitationId": "c53ad41d-8b71-56a6-b333-791e8e371e38",
          "captionText": "FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588711/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=c53ad41d-8b71-56a6-b333-791e8e371e38"
            }
          }
        },
        {
          "figureCitationId": "028e4a8c-3ec9-5585-a0ad-7642fcfe2425",
          "captionText": "FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588711/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=028e4a8c-3ec9-5585-a0ad-7642fcfe2425"
            }
          }
        },
        {
          "figureCitationId": "82362947-9248-5d4c-b8af-36fa67b33dad",
          "captionText": "FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588711/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=82362947-9248-5d4c-b8af-36fa67b33dad"
            }
          }
        },
        {
          "figureCitationId": "a877f39d-bcc3-5d62-9300-f4dfe7b6ca72",
          "captionText": "FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.",
          "httpUri": "https://zenodo.org/record/2588715/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=a877f39d-bcc3-5d62-9300-f4dfe7b6ca72"
            }
          }
        },
        {
          "figureCitationId": "294f4e49-50ec-52da-a3d6-0ecc70ea4cf2",
          "captionText": "FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588711/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=294f4e49-50ec-52da-a3d6-0ecc70ea4cf2"
            }
          }
        },
        {
          "figureCitationId": "60d051b9-6fa3-58e3-b443-92f137e4df58",
          "captionText": "FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.",
          "httpUri": "https://zenodo.org/record/2588715/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=60d051b9-6fa3-58e3-b443-92f137e4df58"
            }
          }
        },
        {
          "figureCitationId": "1c8e1faf-6a89-53fe-8b8c-5a4d0476bf50",
          "captionText": "FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.",
          "httpUri": "https://zenodo.org/record/2588715/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=1c8e1faf-6a89-53fe-8b8c-5a4d0476bf50"
            }
          }
        },
        {
          "figureCitationId": "666e39d2-2c4f-5297-b9e7-e2f576929e20",
          "captionText": "FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.",
          "httpUri": "https://zenodo.org/record/2588715/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=666e39d2-2c4f-5297-b9e7-e2f576929e20"
            }
          }
        },
        {
          "figureCitationId": "8912c092-34d6-54b9-98d5-9701069c9b12",
          "captionText": "FIGURE 20. Habitus images of living paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, anterior view; B, dorsal view; C, lateral view; D: anterolateral view; E, dorsolateral view; F, lateral view.",
          "httpUri": "https://zenodo.org/record/2588711/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=8912c092-34d6-54b9-98d5-9701069c9b12"
            }
          }
        },
        {
          "figureCitationId": "06fee1b1-e942-57cc-b40d-52ee28a35f0d",
          "captionText": "FIGURE 21. Habitus and epigyne images of preserved paratype 1 female Maratus felinus sp. nov. (WAM-T147354): A, ventral view; B, lateral view; C, dorsal view; D, ventral view of epigyne.",
          "httpUri": "https://zenodo.org/record/2588715/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=06fee1b1-e942-57cc-b40d-52ee28a35f0d"
            }
          }
        },
        {
          "figureCitationId": "f3f809b8-9a40-5fa8-9d10-3d2e2a40bf31",
          "captionText": "FIGURE 22. Variation in preserved holotype and paratype male Maratus felinus sp. nov. specimens: A, holotype male; B, paratype male 1.",
          "httpUri": "https://zenodo.org/record/2588717/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=f3f809b8-9a40-5fa8-9d10-3d2e2a40bf31"
            }
          }
        },
        {
          "figureCitationId": "a77ab2de-1f04-5e2d-bc65-ba483a0743eb",
          "captionText": "FIGURE 23. Variation in preserved paratype male Maratus felinus sp. nov. specimens: A, paratype female 1; B, paratype female 2.",
          "httpUri": "https://zenodo.org/record/2588719/files/figure.png",
          "thumbnailUri": "",
          "_links": {
            "self": {
              "href": "https://zenodeo.punkish.org/v2/figurecitations?figureCitationId=a77ab2de-1f04-5e2d-bc65-ba483a0743eb"
            }
          }
        }
      ]
    }
  },
  "cached": null,
  "report": {
    "msec": 0.2926301956176758
  }
}
```
### Search result display

* treatmentTitle
* publication info = *articleTitle* + journalTitle + journalVolume + journalIssue + journalYear + *articleDoi* + *articlePages* + pages
* status
* link to zenodo record = doi
* link to treatmentbank = "http://treatment.plazi.org/id/" + treatmentID
* image count = count(figureCitations items)
* materials count = count(materialsCitations items)


### Treatment page display
