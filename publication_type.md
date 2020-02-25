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
{
	"value": {
		"search-criteria": {
			"page": "1",
			"q": "carabus",
			"size": "30"
		},
		"num-of-records": 34,
		"records": [
			{
				"conceptrecid": "781922",
				"created": "2017-05-12T14:16:03.545130+00:00",
				"doi": "10.3897/zookeys.1.13",
				"files": [
					{
						"bucket": "15717c7a-c1f7-47e7-81e5-ee2e9a425b86",
						"checksum": "md5:30821d7b54ffbe3c93cf9fc75f63f619",
						"key": "ZK_article_1926.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/15717c7a-c1f7-47e7-81e5-ee2e9a425b86/ZK_article_1926.pdf"
						},
						"size": 1781644,
						"type": "pdf"
					}
				],
				"id": 576393,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.1.13.svg",
					"bucket": "https://zenodo.org/api/files/15717c7a-c1f7-47e7-81e5-ee2e9a425b86",
					"doi": "https://doi.org/10.3897/zookeys.1.13",
					"html": "https://zenodo.org/record/576393",
					"latest": "https://zenodo.org/api/records/576393",
					"latest_html": "https://zenodo.org/record/576393",
					"self": "https://zenodo.org/api/records/576393"
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
							"affiliation": "Institute of Ecology, University of Lüneburg, Lüneburg, Lüneburg, Germany",
							"name": "Assmann, Thorsten"
						},
						{
							"affiliation": ", , Germany",
							"name": "Buse, Jörn"
						},
						{
							"affiliation": "University of Lueneburg, Lueneberg, Germany",
							"name": "Drees, Claudia"
						},
						{
							"affiliation": "Tel Aviv University, , Israel",
							"name": "Friedman, Ariel-Leib-Leonid"
						},
						{
							"affiliation": "Department of Zoology, Tel Aviv University, Tel Aviv, , Israel",
							"name": "Levanony, Tal"
						},
						{
							"affiliation": "Institute of Ecology and Environmental Chemistry, University of Lüneburg, Lüneburg, , Germany",
							"name": "Matern, Andrea"
						},
						{
							"affiliation": "Institute of Ecology and Environmental Chemistry, University of Lüneburg, Lüneburg, , Germany",
							"name": "Timm, Anika"
						},
						{
							"affiliation": ", , Germany",
							"name": "Wrase, David"
						}
					],
					"description": "<p>This key to the <em>Carabus</em> species of Israel is an updated identification key with notes on the distribution and habitats of the species. Substantial additions, corrections and taxonomic changes on the <em>Carabus</em> fauna of the Middle East generated the need of an of the knowledge of the genus <em>Carabus</em> in Israel. The classification and the identification of sibling taxa of the subgenus <em>Lamprostus</em> are still a problem: A zone of sympatry supports the species status of both <em>C. sidonius</em> and <em>C. hemprichi</em>. The lack of any evidence of sympatry for the taxa in species rank of the <em>C. syrus</em> group and their variability of the exoskeleton (mentum tooth, tip of aedeagus) requires further systematic and taxonomic studies.</p>",
					"doi": "10.3897/zookeys.1.13",
					"journal": {
						"issue": "",
						"pages": "9-22",
						"title": "ZooKeys",
						"volume": "1"
					},
					"keywords": [
						"Carabus",
						"Lamprostus",
						"identifi cation key",
						"faunistical records",
						"habitat characteristics",
						"Israel"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2008-07-04",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "576393"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "781922"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "The Carabus fauna of Israel – updated identification key, faunistics, and habitats (Coleoptera: Carabidae)"
				},
				"owners": [
					1161
				],
				"revision": 8,
				"stats": {
					"downloads": 12,
					"unique_downloads": 11,
					"unique_views": 7,
					"version_downloads": 12,
					"version_unique_downloads": 11,
					"version_unique_views": 8,
					"version_views": 8,
					"version_volume": 21379728,
					"views": 7,
					"volume": 21379728
				},
				"updated": "2020-01-20T13:33:27.299908+00:00"
			},
			{
				"conceptrecid": "2427021",
				"created": "2018-12-19T16:25:01.301704+00:00",
				"doi": "10.1002/mmnd.192119210409",
				"files": [
					{
						"bucket": "bf91d630-7bbd-4aa0-b3ef-08fea220e163",
						"checksum": "md5:43e208a9048a98da45133e56cb262197",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/bf91d630-7bbd-4aa0-b3ef-08fea220e163/article.pdf"
						},
						"size": 117525,
						"type": "pdf"
					}
				],
				"id": 2427022,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1002/mmnd.192119210409.svg",
					"bucket": "https://zenodo.org/api/files/bf91d630-7bbd-4aa0-b3ef-08fea220e163",
					"doi": "https://doi.org/10.1002/mmnd.192119210409",
					"html": "https://zenodo.org/record/2427022",
					"latest": "https://zenodo.org/api/records/2427022",
					"latest_html": "https://zenodo.org/record/2427022",
					"self": "https://zenodo.org/api/records/2427022"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Reineck, G."
						}
					],
					"description": "n/a",
					"doi": "10.1002/mmnd.192119210409",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1921-01-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "2427022"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "2427021"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Carabus granulatus L. und menetriesi Humm"
				},
				"owners": [
					13380
				],
				"revision": 5,
				"stats": {
					"downloads": 19,
					"unique_downloads": 18,
					"unique_views": 5,
					"version_downloads": 19,
					"version_unique_downloads": 18,
					"version_unique_views": 5,
					"version_views": 5,
					"version_volume": 2232975,
					"views": 5,
					"volume": 2232975
				},
				"updated": "2020-01-20T14:05:00.986671+00:00"
			},
			{
				"conceptrecid": "784347",
				"created": "2017-05-12T16:55:14.135573+00:00",
				"doi": "10.3897/zookeys.463.8499",
				"files": [
					{
						"bucket": "63990856-f468-45ab-b3e2-0a208e22f292",
						"checksum": "md5:0578acbb5e458c896da14521e3ccae0b",
						"key": "ZK_article_4322.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/63990856-f468-45ab-b3e2-0a208e22f292/ZK_article_4322.pdf"
						},
						"size": 21609281,
						"type": "pdf"
					},
					{
						"bucket": "63990856-f468-45ab-b3e2-0a208e22f292",
						"checksum": "md5:375be7f6732db4eec5c39926a2f6219d",
						"key": "ZK_article_4322.xml",
						"links": {
							"self": "https://zenodo.org/api/files/63990856-f468-45ab-b3e2-0a208e22f292/ZK_article_4322.xml"
						},
						"size": 241346,
						"type": "xml"
					}
				],
				"id": 578654,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.463.8499.svg",
					"bucket": "https://zenodo.org/api/files/63990856-f468-45ab-b3e2-0a208e22f292",
					"doi": "https://doi.org/10.3897/zookeys.463.8499",
					"html": "https://zenodo.org/record/578654",
					"latest": "https://zenodo.org/api/records/578654",
					"latest_html": "https://zenodo.org/record/578654",
					"self": "https://zenodo.org/api/records/578654"
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
							"affiliation": "Vitebsk State P.M. Masherov University, Vitebsk, Belarus",
							"name": "Solodovnikov, Igor A."
						},
						{
							"affiliation": "Kuban State Agrarian University, Krasnodar, Russia",
							"name": "Zamotajlov, Alexandr S."
						},
						{
							"affiliation": "Russian Entomological Society, Kuban Branch, Krasnodar, Russia",
							"name": "Fominykh, Dmitriy D."
						},
						{
							"affiliation": "Publicly Traded Company \"Morpho Absoloni\", Moscow, Russia",
							"name": "Titarenko, Andrey Y."
						}
					],
					"description": "<p>This study is based on a comparative analysis of extensive material of Carabus (Archiplectes) satyrus Kurnakov, 1962, its various forms and related taxa recently collected by the authors and some other collectors in Abkhazia. The status or specific affiliations of several subspecies are changed and a subspecies is described. Carabus (A.) besleticus Kurnakov, 1972, stat. n. is treated as a separate species housing six hitherto established subspecies in addition to the nominal type: C. (A.) besleticus mtsaranus Kurnakov, 1972, C. (A.) besleticus duripshensis Kurnakov, 1972, C. (A.) besleticus napraensis Belousov &amp; Zamotajlov, 1993, C. (A.) besleticus dsychvensis Kurnakov, 1972, C. (A.) besleticus adzinbai Retezár, 2013, and C. (A.) besleticus resheviensis subsp. n. Carabus (A.) satyrus is treated as monotypical while the specific status of C. (A.) pseudopshuensis Zamotajlov, 1991, earlier proposed by Fominykh and Zamotajlov (2012), is confirmed based on the morphological and morphometric data.</p>",
					"doi": "10.3897/zookeys.463.8499",
					"journal": {
						"issue": "",
						"pages": "21-56",
						"title": "ZooKeys",
						"volume": "463"
					},
					"keywords": [
						"Animalia",
						"Arthropoda",
						"Insecta",
						"Coleoptera",
						"Caraboidea",
						"Carabidae",
						"Carabus",
						"Carabus satyrusAnimalia",
						"ColeopteraAnimalia",
						"Coleoptera",
						"Carabidae",
						"Carabus (Archiplectes) satyrus species complex",
						"Abkhazia",
						"taxonomy",
						"distribution",
						"new status",
						"new subspecies"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2014-12-12",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "578654"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "784347"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Contribution to the knowledge of the Carabus (Archiplectes) satyrus Kurnakov, 1962, species complex in Abkhazia (Coleoptera, Carabidae, Carabini)"
				},
				"owners": [
					1161
				],
				"revision": 7,
				"stats": {
					"downloads": 5,
					"unique_downloads": 5,
					"unique_views": 7,
					"version_downloads": 5,
					"version_unique_downloads": 5,
					"version_unique_views": 7,
					"version_views": 7,
					"version_volume": 108046405,
					"views": 7,
					"volume": 108046405
				},
				"updated": "2020-01-20T15:00:17.673193+00:00"
			},
			{
				"conceptrecid": "1897177",
				"created": "2018-12-03T23:10:53.949285+00:00",
				"doi": "10.1002/mmnd.192219220312",
				"files": [
					{
						"bucket": "4636caea-7b8f-464e-85e5-b02aabb3107b",
						"checksum": "md5:a3ed80042738fe59ae5b161ab1731e92",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/4636caea-7b8f-464e-85e5-b02aabb3107b/article.pdf"
						},
						"size": 127016,
						"type": "pdf"
					}
				],
				"id": 1897178,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1002/mmnd.192219220312.svg",
					"bucket": "https://zenodo.org/api/files/4636caea-7b8f-464e-85e5-b02aabb3107b",
					"doi": "https://doi.org/10.1002/mmnd.192219220312",
					"html": "https://zenodo.org/record/1897178",
					"latest": "https://zenodo.org/api/records/1897178",
					"latest_html": "https://zenodo.org/record/1897178",
					"self": "https://zenodo.org/api/records/1897178"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Schumacher, F."
						}
					],
					"description": "n/a",
					"doi": "10.1002/mmnd.192219220312",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1922-01-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1897178"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1897177"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Kommt Carabus auratus L. in Ostpreußen vor?"
				},
				"owners": [
					13380
				],
				"revision": 8,
				"stats": {
					"downloads": 22,
					"unique_downloads": 21,
					"unique_views": 5,
					"version_downloads": 22,
					"version_unique_downloads": 21,
					"version_unique_views": 4,
					"version_views": 4,
					"version_volume": 2794352,
					"views": 5,
					"volume": 2794352
				},
				"updated": "2020-01-20T17:08:56.366245+00:00"
			},
			{
				"conceptdoi": "10.5281/zenodo.2521181",
				"conceptrecid": "2521181",
				"created": "2018-12-23T05:07:17.072610+00:00",
				"doi": "10.5281/zenodo.2521182",
				"files": [
					{
						"bucket": "e10a0fc4-4463-458b-b836-ed9e9c1c0afe",
						"checksum": "md5:24f7659f8549c04281a75d95504e8486",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/e10a0fc4-4463-458b-b836-ed9e9c1c0afe/article.pdf"
						},
						"size": 2495257,
						"type": "pdf"
					}
				],
				"id": 2521182,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.5281/zenodo.2521182.svg",
					"bucket": "https://zenodo.org/api/files/e10a0fc4-4463-458b-b836-ed9e9c1c0afe",
					"conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.2521181.svg",
					"conceptdoi": "https://doi.org/10.5281/zenodo.2521181",
					"doi": "https://doi.org/10.5281/zenodo.2521182",
					"html": "https://zenodo.org/record/2521182",
					"latest": "https://zenodo.org/api/records/2521182",
					"latest_html": "https://zenodo.org/record/2521182",
					"self": "https://zenodo.org/api/records/2521182"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Frost, C. A."
						}
					],
					"description": "Volume: 17 ; Start Page: 86 ; End Page: 86",
					"doi": "10.5281/zenodo.2521182",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1910-01-01",
					"related_identifiers": [
						{
							"identifier": "10.5281/zenodo.2521181",
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
									"pid_value": "2521182"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "2521181"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "On the Repugnatorial Secretion of Carabus Vinctus"
				},
				"owners": [
					13380
				],
				"revision": 6,
				"stats": {
					"downloads": 18,
					"unique_downloads": 17,
					"unique_views": 5,
					"version_downloads": 18,
					"version_unique_downloads": 17,
					"version_unique_views": 5,
					"version_views": 5,
					"version_volume": 44914626,
					"views": 5,
					"volume": 44914626
				},
				"updated": "2020-01-20T13:32:21.799662+00:00"
			},
			{
				"conceptrecid": "3406922",
				"created": "2019-09-13T04:30:55.222728+00:00",
				"doi": "10.3897/aca.2.e46305",
				"files": [
					{
						"bucket": "6de99f0a-cc2a-4918-8566-b4b913f73966",
						"checksum": "md5:6a7b0ebecfe2d26f33289ee2eee932d1",
						"key": "ACA_article_46305.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/6de99f0a-cc2a-4918-8566-b4b913f73966/ACA_article_46305.pdf"
						},
						"size": 64683,
						"type": "pdf"
					},
					{
						"bucket": "6de99f0a-cc2a-4918-8566-b4b913f73966",
						"checksum": "md5:cba2a61777925d32ff7e8796d850a573",
						"key": "ACA_article_46305.xml",
						"links": {
							"self": "https://zenodo.org/api/files/6de99f0a-cc2a-4918-8566-b4b913f73966/ACA_article_46305.xml"
						},
						"size": 6141,
						"type": "xml"
					}
				],
				"id": 3406923,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e46305.svg",
					"bucket": "https://zenodo.org/api/files/6de99f0a-cc2a-4918-8566-b4b913f73966",
					"doi": "https://doi.org/10.3897/aca.2.e46305",
					"html": "https://zenodo.org/record/3406923",
					"latest": "https://zenodo.org/api/records/3406923",
					"latest_html": "https://zenodo.org/record/3406923",
					"self": "https://zenodo.org/api/records/3406923"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Duna-Ipoly National Park, Budapest, Hungary",
							"name": "Sándor, Bérces"
						}
					],
					"description": "<p>A two season capture-recapture study was preformed between 2016-2017, focusing on the <em>Carabus </em>species living in a suburban park (3 hectare) in Budapest, Hungary. Eighty live-capture, non-baited pitfall traps were used in a 3 x 3 m grid in 4 rows and 20 columns, covering almost totally a forested area of 240 m2. Five <em>Carabus </em>species were captured, the most numerous were C. scheidleri, <em>C. ullrichii</em> and <em>C. coriaceus</em>. <em>C. convexus</em> and <em>C. intricatus</em> were captured only a few times. All <em>Carabus </em>species were individually marked and released. Population size and survival rate was estimated only for the <em>C. scheidleri</em> population using POPAN in order to receive gross population size. In total 491 <em>C. scheidleri</em> individuals (251 females and 239 males) were marked. Recapture rate in 2016 and 2017 were 41 and 50 percent for the total population respectively. Estimated population size varied between years, the maximum population size was 680 ± 50 specimen in 2016. In 2017 a population size of 190 ± 16 individuals were estimated. Overwintering of eight <em>C. scheidleri</em> and three <em>C. ullrichii</em> specimen were observed. Less mobile large bodied forest specialist <em>Carabus </em>species living in a relatively small reserve underline the importance of habitat islands in a city.</p>",
					"doi": "10.3897/aca.2.e46305",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e46305",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"urbanisation",
						"Carabus scheidleri",
						"mark-recapture",
						"Carabus species",
						"nature reserve",
						"Hungary"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-09-05",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3406923"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3406922"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Does a suburban reserve host a significant Carabuspopulations? A capture-recapture case study in Budapest, Hungary"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 15,
					"unique_downloads": 9,
					"unique_views": 4,
					"version_downloads": 15,
					"version_unique_downloads": 9,
					"version_unique_views": 4,
					"version_views": 4,
					"version_volume": 736077,
					"views": 4,
					"volume": 736077
				},
				"updated": "2020-01-20T16:49:51.518036+00:00"
			},
			{
				"conceptrecid": "784451",
				"created": "2017-05-12T17:08:48.351875+00:00",
				"doi": "10.3897/zookeys.496.9428",
				"files": [
					{
						"bucket": "66371da6-5a56-4b59-bf18-d9d3b4f283af",
						"checksum": "md5:b8cf9b59d79951088ee44fd48c36e0ca",
						"key": "ZK_article_5107.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/66371da6-5a56-4b59-bf18-d9d3b4f283af/ZK_article_5107.pdf"
						},
						"size": 6680189,
						"type": "pdf"
					},
					{
						"bucket": "66371da6-5a56-4b59-bf18-d9d3b4f283af",
						"checksum": "md5:91f36874e6b329b5a756261a45cc107d",
						"key": "ZK_article_5107.xml",
						"links": {
							"self": "https://zenodo.org/api/files/66371da6-5a56-4b59-bf18-d9d3b4f283af/ZK_article_5107.xml"
						},
						"size": 166839,
						"type": "xml"
					}
				],
				"id": 578810,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.496.9428.svg",
					"bucket": "https://zenodo.org/api/files/66371da6-5a56-4b59-bf18-d9d3b4f283af",
					"doi": "https://doi.org/10.3897/zookeys.496.9428",
					"html": "https://zenodo.org/record/578810",
					"latest": "https://zenodo.org/api/records/578810",
					"latest_html": "https://zenodo.org/record/578810",
					"self": "https://zenodo.org/api/records/578810"
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
							"affiliation": "Istituto Zooprofilattico Sperimentale Umbria-Marche, Terni, Italy",
							"name": "Ghittino, Claudio"
						},
						{
							"affiliation": "University of Turin, Torino, Italy",
							"name": "Busato, Enrico"
						},
						{
							"affiliation": "Universitа di Sassari, Sassari, Italy",
							"name": "Casale, Achille"
						}
					],
					"description": "<p>Carabus (Cathoplius) aliai was described as a separate species by Escalera in 1944 but since the 1950–60s it has been considered as a subspecies of C. (Cathoplius) stenocephalus Lucas, 1866. This downgrading was adopted after examining only a few specimens, due to their rarity in collections. In recent years, an important population of this taxon was rediscovered in the Tan-Tan area in southern Morocco. By combining field observations with laboratory breeding experiments including hybridization trials, and through the morphological examination of a representative number of individuals, it is confirmed that C. aliai is indeed a valid species. Despite close geographic distribution, the morphological and biological characteristics of C. aliai and C. stenocephalus ifniensis Zarco, 1941, its northern substitutive taxon, are very different. Carabus aliai adults are characterized by a smaller size, a slender silhouette, a more brilliant aspect, a narrower pronotum, a coarser elytral sculpture, longer legs, and a wider and a little more curved apex of the median lobe of the aedeagus. Carabus aliai larvae are also characterized by a much smaller size and the C. aliai pupa has a narrower thoracic area and a different chaetotaxy compared to that of C. stenocephalus ifniensis. Contrary to this, C. aliai has a life cycle belonging to the annual univoltine winter semelparous type. Moreover, the duration of its development cycle is shorter. Carabus aliai is a sabulicolous steppe-wandering species with an intensive running activity, while C. stenocephalus ifniensis is a more sedentary taxon. Crossbreeding experiments showed a marked reproductive isolation between C. aliai and C. stenocephalus ifniensis. When F1 hybrids were crossed with one another, a very high mortality rate during embryonic, larval and pupal development was evident and no vital F2 neo-adults were obtained. Morphological and biological differences, together with the reproductive failure in C. aliai × C. stenocephalus ifniensis hybrids, clearly indicate that C. aliai is a separate Cathoplius species that is distributed in an area south of the Anti-Atlas chain, from Plage Blanche (Guelmim) to Lemsid and Bou Kra (south of Laâyoune). Carabus aliai is therefore both a Saharan desert endemic and an Atlantic resident. Moreover, it is the southernmost Carabus species of the western Palaearctic region.</p>",
					"doi": "10.3897/zookeys.496.9428",
					"journal": {
						"issue": "",
						"pages": "61-84",
						"title": "ZooKeys",
						"volume": "496"
					},
					"keywords": [
						"Animalia",
						"Arthropoda",
						"Insecta",
						"Coleoptera",
						"Caraboidea",
						"Carabidae",
						"CarabusCarabusCephalornis",
						"Coelenterata",
						"Bilateria",
						"Nephrozoa",
						"Protostomia",
						"Ecdysozoa",
						"Circumscriptional names of the taxon under",
						"Notchia",
						"Carbotriplurida",
						"Boltonocostidae",
						"Circumscriptional names",
						"Pterygota",
						"Pharotarsus",
						"Protodytiscus",
						"Abacaelostus",
						"Carabinae",
						"Calosoma maximoviczi",
						"Carabus ustulatus",
						"CarabusCephalornis",
						"Carabus",
						"CarabusAnimalia",
						"ColeopteraAnimalia",
						"Carabus ground beetles",
						"Saharan desert endemism",
						"Atlantic element",
						"life cycle",
						"hybridization"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2015-04-16",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "578810"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "784451"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Re-establishment of Carabus (Cathoplius) aliai Escalera, 1944 as a separate valid species (Coleoptera, Carabidae)"
				},
				"owners": [
					1161
				],
				"revision": 7,
				"stats": {
					"downloads": 5,
					"unique_downloads": 5,
					"unique_views": 9,
					"version_downloads": 5,
					"version_unique_downloads": 5,
					"version_unique_views": 9,
					"version_views": 10,
					"version_volume": 33400945,
					"views": 10,
					"volume": 33400945
				},
				"updated": "2020-01-20T17:12:10.454824+00:00"
			},
			{
				"conceptrecid": "3250451",
				"created": "2019-06-20T04:30:52.042237+00:00",
				"doi": "10.3897/aca.2.e37128",
				"files": [
					{
						"bucket": "01088659-3e5c-4b43-a755-651ca18aa6b9",
						"checksum": "md5:c51fb07eb3e029d80f573f4998d6eaf8",
						"key": "ACA_article_37128.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/01088659-3e5c-4b43-a755-651ca18aa6b9/ACA_article_37128.pdf"
						},
						"size": 58396,
						"type": "pdf"
					},
					{
						"bucket": "01088659-3e5c-4b43-a755-651ca18aa6b9",
						"checksum": "md5:a701be73b755a3f25d8ef81867db1183",
						"key": "ACA_article_37128.xml",
						"links": {
							"self": "https://zenodo.org/api/files/01088659-3e5c-4b43-a755-651ca18aa6b9/ACA_article_37128.xml"
						},
						"size": 6633,
						"type": "xml"
					}
				],
				"id": 3250452,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e37128.svg",
					"bucket": "https://zenodo.org/api/files/01088659-3e5c-4b43-a755-651ca18aa6b9",
					"doi": "https://doi.org/10.3897/aca.2.e37128",
					"html": "https://zenodo.org/record/3250452",
					"latest": "https://zenodo.org/api/records/3250452",
					"latest_html": "https://zenodo.org/record/3250452",
					"self": "https://zenodo.org/api/records/3250452"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Institute of Zoology, Hamburg, Germany",
							"name": "Drees, Claudia"
						},
						{
							"affiliation": "University of Sussex, Falmer, Brighton, United Kingdom",
							"name": "Schuett, Wiebke"
						},
						{
							"affiliation": "University of Sussex, Falmer, Brighton, United Kingdom",
							"name": "Yarwood, Elisabeth"
						},
						{
							"affiliation": "Leuphana Universitat, Luneburg, Germany",
							"name": "Assmann, Thorsten"
						}
					],
					"description": "<p>Individuals need to find both suitable environmental conditions and mating partners which might be especially difficult for solitary species. Here, we experimentally studied the role of olfactory cues in attracting conspecifics in several forest-dwelling <em>Carabus </em>species. We considered two possible ways of attraction, general aggregation and sexual attraction. In a field experiment we used single male and female beetles as baits in dry pitfall traps and compared the catches of these traps to those in empty ones. Depending on the species, we found suggestive evidence for aggregation behaviour and/or sexual attraction. Our study highlights that olfactory cues play an important role in <em>Carabus</em> but the underlying mechanisms remain to be studied.</p>",
					"doi": "10.3897/aca.2.e37128",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e37128",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-06-12",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3250452"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3250451"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Aggregation and sexual attraction in Carabus – a field experiment"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 8,
					"unique_downloads": 8,
					"unique_views": 9,
					"version_downloads": 8,
					"version_unique_downloads": 8,
					"version_unique_views": 9,
					"version_views": 9,
					"version_volume": 467168,
					"views": 9,
					"volume": 467168
				},
				"updated": "2020-01-20T15:36:26.548599+00:00"
			},
			{
				"conceptrecid": "3256872",
				"created": "2019-06-26T04:35:43.042520+00:00",
				"doi": "10.3897/aca.2.e37362",
				"files": [
					{
						"bucket": "ddd5e022-d917-4be9-9947-002a6d5010d9",
						"checksum": "md5:36f26368de92c94bd1c6c12a80c1e5fc",
						"key": "ACA_article_37362.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/ddd5e022-d917-4be9-9947-002a6d5010d9/ACA_article_37362.pdf"
						},
						"size": 65063,
						"type": "pdf"
					},
					{
						"bucket": "ddd5e022-d917-4be9-9947-002a6d5010d9",
						"checksum": "md5:830c42c036022cd1c41a8e7430176300",
						"key": "ACA_article_37362.xml",
						"links": {
							"self": "https://zenodo.org/api/files/ddd5e022-d917-4be9-9947-002a6d5010d9/ACA_article_37362.xml"
						},
						"size": 9035,
						"type": "xml"
					}
				],
				"id": 3256873,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e37362.svg",
					"bucket": "https://zenodo.org/api/files/ddd5e022-d917-4be9-9947-002a6d5010d9",
					"doi": "https://doi.org/10.3897/aca.2.e37362",
					"html": "https://zenodo.org/record/3256873",
					"latest": "https://zenodo.org/api/records/3256873",
					"latest_html": "https://zenodo.org/record/3256873",
					"self": "https://zenodo.org/api/records/3256873"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Seeweg 10, 23942 Gross Schwansee, Germany",
							"name": "Mossakowski, Dietrich"
						},
						{
							"affiliation": "AOPK ČR, Kaplanova 1931/1, 148 00 Praha 11 – Chodov, Czech Republic",
							"name": "Hejda, Radek"
						},
						{
							"affiliation": "Bavarian LWF, Hans-Carl-von-Carlowitz-Platz 1, 85354 Freising, Germany",
							"name": "Müller-Kroehling, Stefan"
						},
						{
							"affiliation": "Studienzentrum Naturkunde, Weinzöttlstraße 16, 8045 Graz, Austria",
							"name": "Paill, Wolfgang"
						},
						{
							"affiliation": "Banat's University of Agricultural Sciences and Veterinary Medicine, 119 Calea Aradului, 300645 Timisoara, Romania",
							"name": "Prunar, Florin"
						},
						{
							"affiliation": "Via Cialla, 47, 33040 Prepotto (UD), Italy",
							"name": "Rapuzzi, Ivan"
						}
					],
					"description": "<p>Starting point of this study was the problem considering the status of <em>Carabus variolous</em> and <em>C. nodulosus</em>: French and some German authors classified them as species, most German authors as subspecies and Casale as semispecies.</p>\n  <p>We performed analyses of mitochondrial genes (COI-5', COI-3', ND5) as well as nuclear ones (ITS2, wingless) and analysed the DNA sequences using Seqotron, CLUSTALX (editing and alignment), MEGA, DNAML, SplitsTree (phylogeny and network), 4SALE (compensatory base changes), and BEAST (coalescence).</p>\n  <p>We could study specimens from all regions except the western most part of the distribution area (Massif Central and French Jura, France).</p>\n  <p>The mitochondrial DNA data resulted in a geographic pattern of high diversity within both taxa indicating a series of glacial refuges. In addition, a considerably large area was found were introgressive hybridisation took place in the past - at least two times by nodulosus of different regions into variolosus. </p>\n  <p>The nuclear DNA data show a clear and constant difference between both taxa. </p>\n  <p>In consequence, this complex of forms may be characterised as semispecies from an evolutionary viewpoint but taxonomically as one species because of  hybridisation and the lack of compensatory bases changes.</p>",
					"doi": "10.3897/aca.2.e37362",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e37362",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"Species status",
						"introgressive hybridisation",
						"multiple refuges"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-06-18",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3256873"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3256872"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "High molecular diversity in the Carabus variolosus/nodulosus complex"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 8,
					"unique_downloads": 8,
					"unique_views": 20,
					"version_downloads": 8,
					"version_unique_downloads": 8,
					"version_unique_views": 20,
					"version_views": 20,
					"version_volume": 520504,
					"views": 20,
					"volume": 520504
				},
				"updated": "2020-01-20T16:17:29.933566+00:00"
			},
			{
				"conceptrecid": "2303801",
				"created": "2018-12-15T22:57:43.264464+00:00",
				"doi": "10.1080/037454809496004",
				"files": [
					{
						"bucket": "8843aa83-4696-46df-a2b3-2dd763e93209",
						"checksum": "md5:9ea22e2284637fc89c2495c60ad0b9eb",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/8843aa83-4696-46df-a2b3-2dd763e93209/article.pdf"
						},
						"size": 360321,
						"type": "pdf"
					}
				],
				"id": 2303802,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1080/037454809496004.svg",
					"bucket": "https://zenodo.org/api/files/8843aa83-4696-46df-a2b3-2dd763e93209",
					"doi": "https://doi.org/10.1080/037454809496004",
					"html": "https://zenodo.org/record/2303802",
					"latest": "https://zenodo.org/api/records/2303802",
					"latest_html": "https://zenodo.org/record/2303802",
					"self": "https://zenodo.org/api/records/2303802"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Tatum, T."
						}
					],
					"description": "n/a",
					"doi": "10.1080/037454809496004",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1847-07-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "2303802"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "2303801"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "IV.— Description of two new species of Carabus from Asia"
				},
				"owners": [
					13380
				],
				"revision": 6,
				"stats": {
					"downloads": 17,
					"unique_downloads": 17,
					"unique_views": 3,
					"version_downloads": 17,
					"version_unique_downloads": 17,
					"version_unique_views": 3,
					"version_views": 3,
					"version_volume": 6125457,
					"views": 3,
					"volume": 6125457
				},
				"updated": "2020-01-20T14:08:19.781813+00:00"
			},
			{
				"conceptrecid": "1972712",
				"created": "2018-12-05T14:25:40.308543+00:00",
				"doi": "10.4039/ent37160-5",
				"files": [
					{
						"bucket": "6aff5c93-a7ca-4fe5-81f4-eb8fbaab8544",
						"checksum": "md5:8970e8e80ad47209f4767392ab1ef522",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/6aff5c93-a7ca-4fe5-81f4-eb8fbaab8544/article.pdf"
						},
						"size": 53042,
						"type": "pdf"
					}
				],
				"id": 1972713,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.4039/ent37160-5.svg",
					"bucket": "https://zenodo.org/api/files/6aff5c93-a7ca-4fe5-81f4-eb8fbaab8544",
					"doi": "https://doi.org/10.4039/ent37160-5",
					"html": "https://zenodo.org/record/1972713",
					"latest": "https://zenodo.org/api/records/1972713",
					"latest_html": "https://zenodo.org/record/1972713",
					"self": "https://zenodo.org/api/records/1972713"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Casey, Thos L."
						}
					],
					"description": "n/a",
					"doi": "10.4039/ent37160-5",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1905-05-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1972713"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1972712"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "A New Carabus and Cychrus, With Miscellaneous Notes on Coleoptera"
				},
				"owners": [
					13380
				],
				"revision": 7,
				"stats": {
					"downloads": 29,
					"unique_downloads": 29,
					"unique_views": 8,
					"version_downloads": 29,
					"version_unique_downloads": 29,
					"version_unique_views": 7,
					"version_views": 7,
					"version_volume": 1538218,
					"views": 8,
					"volume": 1538218
				},
				"updated": "2020-01-20T17:35:29.828647+00:00"
			},
			{
				"conceptrecid": "1911560",
				"created": "2018-12-04T05:39:36.572888+00:00",
				"doi": "10.1080/00222938409459770",
				"files": [
					{
						"bucket": "c72ecd51-02ff-4bf2-a7b8-4b24e7cc579b",
						"checksum": "md5:6848a3b08cee75f7dfa5f2ae3d9a4cea",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/c72ecd51-02ff-4bf2-a7b8-4b24e7cc579b/article.pdf"
						},
						"size": 217482,
						"type": "pdf"
					}
				],
				"id": 1911561,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1080/00222938409459770.svg",
					"bucket": "https://zenodo.org/api/files/c72ecd51-02ff-4bf2-a7b8-4b24e7cc579b",
					"doi": "https://doi.org/10.1080/00222938409459770",
					"html": "https://zenodo.org/record/1911561",
					"latest": "https://zenodo.org/api/records/1911561",
					"latest_html": "https://zenodo.org/record/1911561",
					"self": "https://zenodo.org/api/records/1911561"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Cholodkowsky, M. N."
						}
					],
					"description": "n/a",
					"doi": "10.1080/00222938409459770",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1884-07-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1911561"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1911560"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "On a species of Tachina occurring on the tracheal system of Carabus"
				},
				"owners": [
					13380
				],
				"revision": 8,
				"stats": {
					"downloads": 23,
					"unique_downloads": 23,
					"unique_views": 6,
					"version_downloads": 23,
					"version_unique_downloads": 23,
					"version_unique_views": 5,
					"version_views": 5,
					"version_volume": 5002086,
					"views": 6,
					"volume": 5002086
				},
				"updated": "2020-01-20T13:35:38.513724+00:00"
			},
			{
				"conceptrecid": "2192920",
				"created": "2018-12-11T05:50:45.731139+00:00",
				"doi": "10.2307/2331559",
				"files": [
					{
						"bucket": "0384962d-ac57-448b-9478-e8b6ee2360bd",
						"checksum": "md5:77b78626adf669083e9ff46747abc6cf",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/0384962d-ac57-448b-9478-e8b6ee2360bd/article.pdf"
						},
						"size": 362772,
						"type": "pdf"
					}
				],
				"id": 2192921,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.2307/2331559.svg",
					"bucket": "https://zenodo.org/api/files/0384962d-ac57-448b-9478-e8b6ee2360bd",
					"doi": "https://doi.org/10.2307/2331559",
					"html": "https://zenodo.org/record/2192921",
					"latest": "https://zenodo.org/api/records/2192921",
					"latest_html": "https://zenodo.org/record/2192921",
					"self": "https://zenodo.org/api/records/2192921"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Kribs, H. G."
						}
					],
					"description": "n/a",
					"doi": "10.2307/2331559",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1908-03-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "2192921"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "2192920"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Note on the Relative Variability of the Sexes in Carabus Auratus, L"
				},
				"owners": [
					13380
				],
				"revision": 5,
				"stats": {
					"downloads": 20,
					"unique_downloads": 20,
					"unique_views": 6,
					"version_downloads": 20,
					"version_unique_downloads": 20,
					"version_unique_views": 5,
					"version_views": 5,
					"version_volume": 7255440,
					"views": 6,
					"volume": 7255440
				},
				"updated": "2020-01-20T17:31:48.838565+00:00"
			},
			{
				"conceptrecid": "3406920",
				"created": "2019-09-13T04:30:51.323369+00:00",
				"doi": "10.3897/aca.2.e46302",
				"files": [
					{
						"bucket": "15a37c4a-c0b8-4d0b-be0a-c99cb449a1e6",
						"checksum": "md5:947b05b4cf8d10e336d67dff279e6760",
						"key": "ACA_article_46302.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/15a37c4a-c0b8-4d0b-be0a-c99cb449a1e6/ACA_article_46302.pdf"
						},
						"size": 67175,
						"type": "pdf"
					},
					{
						"bucket": "15a37c4a-c0b8-4d0b-be0a-c99cb449a1e6",
						"checksum": "md5:6091ba1a8925d9a163d4395bf7c395dd",
						"key": "ACA_article_46302.xml",
						"links": {
							"self": "https://zenodo.org/api/files/15a37c4a-c0b8-4d0b-be0a-c99cb449a1e6/ACA_article_46302.xml"
						},
						"size": 7589,
						"type": "xml"
					}
				],
				"id": 3406921,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e46302.svg",
					"bucket": "https://zenodo.org/api/files/15a37c4a-c0b8-4d0b-be0a-c99cb449a1e6",
					"doi": "https://doi.org/10.3897/aca.2.e46302",
					"html": "https://zenodo.org/record/3406921",
					"latest": "https://zenodo.org/api/records/3406921",
					"latest_html": "https://zenodo.org/record/3406921",
					"self": "https://zenodo.org/api/records/3406921"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Duna-Ipoly National Park, Budapest, Hungary",
							"name": "Sándor, Bérces"
						},
						{
							"affiliation": "MTA ATK NÖVI, Budapest, Hungary",
							"name": "Fülöp, David"
						},
						{
							"affiliation": "Plant Health and Molecular Biology Laboratory, National Food Chain Safety Office, Directorate of Plant Protection, Soil Conservation and Agri-environment, Budapest, Hungary",
							"name": "Bozsó, Miklós"
						},
						{
							"affiliation": "University of Szeged, Department of Ecology, Szeged, Hungary",
							"name": "Pénzes, Zsolt"
						}
					],
					"description": "<p>The main goal of our study was to analyse the differences between <em>Carabus hungaricus</em> populations in different regions in the Carpathian basin, and to clear the taxonomic rank of the three subspecies living in the area. We performed analyses of mitochondrial genes (COI) to analyse regional isolation besides taxonomic questions. Extensive sampling was preformed spatially, focusing also on the different habitat types hosting <em>C. hungaricus</em> populations. Low differences were found based on mitochondrial genes (COI) between populations living in the Carpathian basin. Neither spatial nor habitat based differences were significant. Some difference were found in the COI sequences from Deliblato sands (Serbia), while significant difference in the COI sequences was found when analysing specimen from the Crimea. The question arises: was there a refugia for <em>Carabus hungaricus</em> within the Carpathian basin in the Ice Ages? To answer this question further research is needed.</p>",
					"doi": "10.3897/aca.2.e46302",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e46302",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"Carabus hungaricus",
						"COI",
						"Carpathian basin"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-09-05",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3406921"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3406920"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Low (COI) differentiation between the Carabus hungaricus populations in the Carpathian basin"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 15,
					"unique_downloads": 9,
					"unique_views": 4,
					"version_downloads": 15,
					"version_unique_downloads": 9,
					"version_unique_views": 4,
					"version_views": 4,
					"version_volume": 769281,
					"views": 4,
					"volume": 769281
				},
				"updated": "2020-01-20T16:49:59.015747+00:00"
			},
			{
				"conceptrecid": "3250449",
				"created": "2019-06-20T04:30:47.756755+00:00",
				"doi": "10.3897/aca.2.e37076",
				"files": [
					{
						"bucket": "e69cefa6-c4b5-48be-acd9-a6d4a0c396f6",
						"checksum": "md5:4d3bac6ae393551fc6c0df254aab45ff",
						"key": "ACA_article_37076.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/e69cefa6-c4b5-48be-acd9-a6d4a0c396f6/ACA_article_37076.pdf"
						},
						"size": 67004,
						"type": "pdf"
					},
					{
						"bucket": "e69cefa6-c4b5-48be-acd9-a6d4a0c396f6",
						"checksum": "md5:adc8222f665e5d9bf0f2e4174f333e46",
						"key": "ACA_article_37076.xml",
						"links": {
							"self": "https://zenodo.org/api/files/e69cefa6-c4b5-48be-acd9-a6d4a0c396f6/ACA_article_37076.xml"
						},
						"size": 7263,
						"type": "xml"
					}
				],
				"id": 3250450,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e37076.svg",
					"bucket": "https://zenodo.org/api/files/e69cefa6-c4b5-48be-acd9-a6d4a0c396f6",
					"doi": "https://doi.org/10.3897/aca.2.e37076",
					"html": "https://zenodo.org/record/3250450",
					"latest": "https://zenodo.org/api/records/3250450",
					"latest_html": "https://zenodo.org/record/3250450",
					"self": "https://zenodo.org/api/records/3250450"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "National Institute of Biology, Ljubljana, Slovenia",
							"name": "Ratajc, Urška"
						},
						{
							"affiliation": "National Institute of Biology, Ljubljana, Slovenia",
							"name": "Kapla, Andrej"
						},
						{
							"affiliation": "National Institute of Biology, Ljubljana, Slovenia",
							"name": "Ambrožič Ergaver, Špela"
						},
						{
							"affiliation": "National Institute of Biology, Ljubljana, Slovenia",
							"name": "Vrezec, Al"
						}
					],
					"description": "<p>In the past few decades, there has been a sharp decline in specialised and rare species of ground beetles (<em>Carabus</em>) throughout Europe. Our aim was to determine the distribution trends of chosen species and their conservation status in Slovenia. Based on historical and recent data over the period from 1850 to 2018, distribution maps for 25 species of genus <em>Carabus</em> have been made. The reduction in distribution area size was used to evaluate the decline of each species in Slovenia and for assigning them to different categories of threat status. Our results show that a significant number of species from genus <em>Carabus</em> are in decline. Open habitat species of ground beetles (<em>C. cancellatus</em>), ground beetles that are dependent on mature, unmanaged forests (<em>C. glabratus, C. croaticus</em>) and species, very sensitive to climate change (<em>C. irregularis</em>) were found to be the most endangered. Currently, only 3 species are on the Red list of threatened species in Slovenia (<em>C. auronitens, C. gigas and C. variolosus nodulosus</em>), and based on our results, at least 10 species of ground beetles should be added to the existing list. Two species of ground beetles, <em>C. kollari</em> and <em>C. montivagus</em>, have already disappeared from Slovenia in the last few decades, therefore intensive ecological studies of the remaining species and immediate effective conservation strategies are essential.</p>",
					"doi": "10.3897/aca.2.e37076",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e37076",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-06-12",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3250450"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3250449"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Distribution changes of Carabusspecies in Slovenia: historical data analysis"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 5,
					"unique_downloads": 5,
					"unique_views": 6,
					"version_downloads": 5,
					"version_unique_downloads": 5,
					"version_unique_views": 6,
					"version_views": 6,
					"version_volume": 335020,
					"views": 6,
					"volume": 335020
				},
				"updated": "2020-01-20T15:34:47.231140+00:00"
			},
			{
				"conceptdoi": "10.5281/zenodo.1108265",
				"conceptrecid": "1108265",
				"created": "2017-12-12T08:37:38.657112+00:00",
				"doi": "10.5281/zenodo.1108266",
				"files": [
					{
						"bucket": "47a3a075-5bc4-4b73-8b7b-0fa2de40b5ad",
						"checksum": "md5:d0aad9d39684d0ac636e7bd2e73dac7c",
						"key": "№19-051-057.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/47a3a075-5bc4-4b73-8b7b-0fa2de40b5ad/%E2%84%9619-051-057.pdf"
						},
						"size": 338320,
						"type": "pdf"
					}
				],
				"id": 1108266,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.5281/zenodo.1108266.svg",
					"bucket": "https://zenodo.org/api/files/47a3a075-5bc4-4b73-8b7b-0fa2de40b5ad",
					"conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.1108265.svg",
					"conceptdoi": "https://doi.org/10.5281/zenodo.1108265",
					"doi": "https://doi.org/10.5281/zenodo.1108266",
					"html": "https://zenodo.org/record/1108266",
					"latest": "https://zenodo.org/api/records/1108266",
					"latest_html": "https://zenodo.org/record/1108266",
					"self": "https://zenodo.org/api/records/1108266"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Дніпровський національний університет імені Олеся Гончара",
							"name": "Ю.Л. Кульбачко",
							"orcid": "0000-0001-9627-3297"
						},
						{
							"affiliation": "Дніпровський національний університет імені Олеся Гончара",
							"name": "О.О. Дідур",
							"orcid": "0000-0001-7425-9013"
						}
					],
					"description": "<p>Morphological variability of soil-inhabiting zoophagous granulated carabid <em>Carabus granulatus </em>Linnaeus, 1758 (Coleoptera, Carabidae) was studied at the site in close proximity to a cement plant (Kamenskoe Cement Plant ―HeidelbergCement Ukraine‖) and at the control site without anthropogenic impact. Statistically significant differences in morphometric features (length and width of head, width and length of pronotum, length and width of elytra, length of antennae) were found. Studied parameters were larger for ground beetles living in the biotopes subjected to the influence of cement production compared to the ones, dwelling the control area. The <em>Carabus granulatus </em>Linnaeus, 1758 species is clearly responsible to changes in livelihoods, including anthropogenic pressure. This is manifested in increasing in the values of morphometric characteristics of individuals. It is established, that the extent of cephalization of ground beetle <em>C. granulatus </em>Linnaeus, 1758 can be used as one of the key signs in bioindication studies.</p>\n\n<p>&nbsp;</p>",
					"doi": "10.5281/zenodo.1108266",
					"journal": {
						"issue": "19",
						"pages": "51-57",
						"title": "Біологія та валеологія"
					},
					"keywords": [
						"ground beetles",
						"Carabus granulates Linnaeus",
						"cement production",
						"morphometry",
						"cephalization"
					],
					"language": "ukr",
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2017-12-12",
					"related_identifiers": [
						{
							"identifier": "10.5281/zenodo.1108265",
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
									"pid_value": "1108266"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1108265"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "МОРФОЛОГІЧНА МІНЛИВІСТЬ ПРЕДСТАВНИКІВ ПЕДОБІОНТІВ- ЗООФАГІВ НА ПРИКЛАДІ CARABUS GRANULATUS LINNAEUS, 1758 (COLEOPTERA, CARABIDAE) В УМОВАХ ТЕХНОГЕННОГО ПРЕСУ"
				},
				"owners": [
					5864
				],
				"revision": 4,
				"stats": {
					"downloads": 9,
					"unique_downloads": 9,
					"unique_views": 13,
					"version_downloads": 9,
					"version_unique_downloads": 9,
					"version_unique_views": 13,
					"version_views": 14,
					"version_volume": 3044880,
					"views": 14,
					"volume": 3044880
				},
				"updated": "2020-01-20T14:45:55.210127+00:00"
			},
			{
				"conceptrecid": "1806155",
				"created": "2018-12-01T16:38:09.316009+00:00",
				"doi": "10.1093/biomet/6.1.103",
				"files": [
					{
						"bucket": "5b0e2092-9f75-4900-94ba-aa8642a6a9d0",
						"checksum": "md5:56efcd2e0016776810c18708ad0c52fe",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/5b0e2092-9f75-4900-94ba-aa8642a6a9d0/article.pdf"
						},
						"size": 165300,
						"type": "pdf"
					}
				],
				"id": 1806156,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1093/biomet/6.1.103.svg",
					"bucket": "https://zenodo.org/api/files/5b0e2092-9f75-4900-94ba-aa8642a6a9d0",
					"doi": "https://doi.org/10.1093/biomet/6.1.103",
					"html": "https://zenodo.org/record/1806156",
					"latest": "https://zenodo.org/api/records/1806156",
					"latest_html": "https://zenodo.org/record/1806156",
					"self": "https://zenodo.org/api/records/1806156"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Kribs, H. G."
						}
					],
					"description": "n/a",
					"doi": "10.1093/biomet/6.1.103",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1908-03-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1806156"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1806155"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "II. Note on the Relative Variability of the Sexes in Carabus auratus, L"
				},
				"owners": [
					13380
				],
				"revision": 6,
				"stats": {
					"downloads": 27,
					"unique_downloads": 27,
					"unique_views": 9,
					"version_downloads": 27,
					"version_unique_downloads": 27,
					"version_unique_views": 8,
					"version_views": 9,
					"version_volume": 4463100,
					"views": 10,
					"volume": 4463100
				},
				"updated": "2020-01-20T14:16:00.343540+00:00"
			},
			{
				"conceptrecid": "1673279",
				"created": "2018-11-29T03:47:16.210588+00:00",
				"doi": "10.1002/prac.18340030158",
				"files": [
					{
						"bucket": "1afdfc5a-1593-4511-b20f-2b61725e04ed",
						"checksum": "md5:b2dda823378f0b7074a8d90ae8b0fc2f",
						"key": "article.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/1afdfc5a-1593-4511-b20f-2b61725e04ed/article.pdf"
						},
						"size": 964480,
						"type": "pdf"
					}
				],
				"id": 1673280,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.1002/prac.18340030158.svg",
					"bucket": "https://zenodo.org/api/files/1afdfc5a-1593-4511-b20f-2b61725e04ed",
					"doi": "https://doi.org/10.1002/prac.18340030158",
					"html": "https://zenodo.org/record/1673280",
					"latest": "https://zenodo.org/api/records/1673280",
					"latest_html": "https://zenodo.org/record/1673280",
					"self": "https://zenodo.org/api/records/1673280"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Hornung, E. G."
						},
						{
							"name": "Blry, L. F."
						}
					],
					"description": "n/a",
					"doi": "10.1002/prac.18340030158",
					"license": {
						"id": "CC0-1.0"
					},
					"publication_date": "1834-01-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1673280"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1673279"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Entomologische-chemische Untersuchung des Carabus auratus L. Goldschmidtkäfers und des Scarabaeus nasicornis L. Nashornkäfers"
				},
				"owners": [
					13380
				],
				"revision": 5,
				"stats": {
					"downloads": 17,
					"unique_downloads": 17,
					"unique_views": 4,
					"version_downloads": 17,
					"version_unique_downloads": 17,
					"version_unique_views": 3,
					"version_views": 3,
					"version_volume": 16396160,
					"views": 4,
					"volume": 16396160
				},
				"updated": "2020-01-20T15:49:11.186115+00:00"
			},
			{
				"conceptrecid": "782538",
				"created": "2017-05-12T14:40:12.263316+00:00",
				"doi": "10.3897/zookeys.100.1546",
				"files": [
					{
						"bucket": "f474e178-26ab-4ca0-a1cc-52450b0ffd2d",
						"checksum": "md5:bd34bba1c6e46d7f39f063434af90680",
						"key": "ZK_article_2363.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/f474e178-26ab-4ca0-a1cc-52450b0ffd2d/ZK_article_2363.pdf"
						},
						"size": 1047437,
						"type": "pdf"
					},
					{
						"bucket": "f474e178-26ab-4ca0-a1cc-52450b0ffd2d",
						"checksum": "md5:9c402cf817c15accfc998b1faa10e006",
						"key": "ZK_article_2363.xml",
						"links": {
							"self": "https://zenodo.org/api/files/f474e178-26ab-4ca0-a1cc-52450b0ffd2d/ZK_article_2363.xml"
						},
						"size": 150880,
						"type": "xml"
					}
				],
				"id": 576820,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.100.1546.svg",
					"bucket": "https://zenodo.org/api/files/f474e178-26ab-4ca0-a1cc-52450b0ffd2d",
					"doi": "https://doi.org/10.3897/zookeys.100.1546",
					"html": "https://zenodo.org/record/576820",
					"latest": "https://zenodo.org/api/records/576820",
					"latest_html": "https://zenodo.org/record/576820",
					"self": "https://zenodo.org/api/records/576820"
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
							"affiliation": "Institute of Ecology and Environmental Chemistry, University of Lüneburg, Lüneburg, , Germany",
							"name": "Matern, Andrea"
						},
						{
							"affiliation": "University of Lueneburg, Lueneberg, Germany",
							"name": "Drees, Claudia"
						},
						{
							"affiliation": "Leuphana University, Lüneburg, Germany",
							"name": "Hardtle, Werner"
						},
						{
							"affiliation": "Institute of Ecology and Environmental Chemistry, Leuphana University, , Germany",
							"name": "von Oheimb, Goddert"
						},
						{
							"affiliation": "Institute of Ecology, University of Lüneburg, Lüneburg, Lüneburg, Germany",
							"name": "Assmann, Thorsten"
						}
					],
					"description": "Only very few cases have documented that an increase in connectivity after a period of fragmentation in ecological time has had an effect on the distribution, genetic structure and morphology of stenotopic species. In this study we present an example of clinal variability in a woodland ground beetle as a result of changes in the connectivity of a landscape during the last two centuries. The study area hosts both the nominate form <i>C. violaceus </i>s. str. and the subspecies <i>C. v.</i> <i>purpurascens</i>, which is ranked as a distinct species by some authors. We studied 12 <i>Carabus violaceus</i> populations from a 30 km transect of ancient and recent forests in north-western Germany. We analyzed three polymorphic enzyme loci, classified the elytron sculpture and measured the shape of the aedeagus tip of the specimens. <i>C. violaceus</i> showed secondary gradients both in allozyme markers and morphometric characters in our study area. A genetic differentiation of 16% between the populations is high but lies within the range of intraspecific variability in habitat specialists of the genus <i>Carabus. </i>Populations had no significant deficit of heterozygotes. We found many hybrid populations in terms of morphological properties. This study highlights the conservation value of ancient woodland and the consequences of landscape connectivity and defragmentation on the genetic setting of a ground beetle. Moreover, it shows that differences in the external shape of male genitalia do not prevent gene flow within the genus <i>Carabus.</i> Thus, the establishment of species status should not exclusively be based on this property.",
					"doi": "10.3897/zookeys.100.1546",
					"journal": {
						"issue": "",
						"pages": "545-563",
						"title": "ZooKeys",
						"volume": "100"
					},
					"keywords": [
						"fragmentation",
						"afforestation",
						"allozymes",
						"morphometrics",
						"Carabus violaceus purpurascens",
						"hybridization",
						"hybrid zone"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2011-05-20",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "576820"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "782538"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Historical ecology meets conservation and evolutionary genetics: a secondary contact zone between Carabus violaceus (Coleoptera, Carabidae) populations inhabiting ancient and recent woodlands in north-western Germany"
				},
				"owners": [
					1161
				],
				"revision": 8,
				"stats": {
					"downloads": 6,
					"unique_downloads": 6,
					"unique_views": 7,
					"version_downloads": 6,
					"version_unique_downloads": 6,
					"version_unique_views": 6,
					"version_views": 6,
					"version_volume": 6284622,
					"views": 7,
					"volume": 6284622
				},
				"updated": "2020-01-20T13:32:46.323430+00:00"
			},
			{
				"conceptdoi": "10.5281/zenodo.3585498",
				"conceptrecid": "3585498",
				"created": "2019-12-19T14:19:00.375881+00:00",
				"doi": "10.5281/zenodo.3585499",
				"files": [
					{
						"bucket": "982b7bc5-8d7d-49e2-9696-8795b5faf2ec",
						"checksum": "md5:c6d476a38738ef2c66219220c711abd7",
						"key": "Ukrentfau_10_2_02_N_Nazarov.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/982b7bc5-8d7d-49e2-9696-8795b5faf2ec/Ukrentfau_10_2_02_N_Nazarov.pdf"
						},
						"size": 2056126,
						"type": "pdf"
					}
				],
				"id": 3585499,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.5281/zenodo.3585499.svg",
					"bucket": "https://zenodo.org/api/files/982b7bc5-8d7d-49e2-9696-8795b5faf2ec",
					"conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.3585498.svg",
					"conceptdoi": "https://doi.org/10.5281/zenodo.3585498",
					"doi": "https://doi.org/10.5281/zenodo.3585499",
					"html": "https://zenodo.org/record/3585499",
					"latest": "https://zenodo.org/api/records/3585499",
					"latest_html": "https://zenodo.org/record/3585499",
					"self": "https://zenodo.org/api/records/3585499"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"name": "Nazarov, N.V."
						}
					],
					"description": "<p>The data on new, rare and local species of ground beetles of the fauna of Ukrainian Polissya are given. Three species (<em>Carabus menetriesi</em> Hummel, <em>Miscodera arctica</em> Paykull, <em>Trechus rivularis</em> Gyllenhal) are found in Ukrainian Polessye on the southern border of the range, one species (C<em>hlaenius spoliatus</em> Rossi) on the northern border of the range, and two species (<em>Agonum hypocrita</em> Apfelbeck, <em>Pterostichus rhaeticus</em> Heer) belong to a taxonomically complex groups of related species, whereas the rest are probably widespread, but rare and local.</p>",
					"doi": "10.5281/zenodo.3585499",
					"journal": {
						"issue": "2",
						"pages": "7-10",
						"title": "Ukrainska Entomofaunistyka",
						"volume": "10"
					},
					"keywords": [
						"ground beetles",
						"Coleoptera",
						"Carabidae",
						"Polesie",
						"Ukraine"
					],
					"language": "rus",
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-12-19",
					"related_identifiers": [
						{
							"identifier": "10.5281/zenodo.3585498",
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
									"pid_value": "3585499"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3585498"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Coleopterological notes"
				},
				"owners": [
					86101
				],
				"revision": 2,
				"stats": {
					"downloads": 30,
					"unique_downloads": 29,
					"unique_views": 35,
					"version_downloads": 30,
					"version_unique_downloads": 29,
					"version_unique_views": 35,
					"version_views": 35,
					"version_volume": 61683780,
					"views": 35,
					"volume": 61683780
				},
				"updated": "2020-01-20T15:47:19.880826+00:00"
			},
			{
				"conceptrecid": "782476",
				"created": "2017-05-12T14:41:54.563977+00:00",
				"doi": "10.3897/zookeys.100.1536",
				"files": [
					{
						"bucket": "6600b775-c346-49da-9eae-bba9246be11d",
						"checksum": "md5:63d00f8c18c10d21219611641de0b2e8",
						"key": "ZK_article_2389.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/6600b775-c346-49da-9eae-bba9246be11d/ZK_article_2389.pdf"
						},
						"size": 986330,
						"type": "pdf"
					},
					{
						"bucket": "6600b775-c346-49da-9eae-bba9246be11d",
						"checksum": "md5:0e262de36a74536913cbd43dbd69ed67",
						"key": "ZK_article_2389.xml",
						"links": {
							"self": "https://zenodo.org/api/files/6600b775-c346-49da-9eae-bba9246be11d/ZK_article_2389.xml"
						},
						"size": 98175,
						"type": "xml"
					}
				],
				"id": 576847,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.100.1536.svg",
					"bucket": "https://zenodo.org/api/files/6600b775-c346-49da-9eae-bba9246be11d",
					"doi": "https://doi.org/10.3897/zookeys.100.1536",
					"html": "https://zenodo.org/record/576847",
					"latest": "https://zenodo.org/api/records/576847",
					"latest_html": "https://zenodo.org/record/576847",
					"self": "https://zenodo.org/api/records/576847"
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
							"affiliation": "Department of Zoology, Faculty of Science, University of Zagreb, Zagreb, Croatia",
							"name": "Šerić Jelaska, Lucija"
						},
						{
							"affiliation": "State Institute for Nature Protection, , Croatia",
							"name": "Dumbovich, Vlatka"
						},
						{
							"affiliation": "State Institute for Nature Protection, , Croatia",
							"name": "Kucinic, Mladen"
						}
					],
					"description": "Carabid beetle diversity and mean individual biomass (MIB) were analysed in three different successional stages of beech tree stands (60, 80 and 150 years old). Carabid beetles were captured using pitfall traps placed at nine sites (three per age class) in the Papuk Mountain of East Croatia during 2008. A cluster analysis identified three groupings that corresponded to the beech age classes. MIB values increased with stand age, ranging from 255 in 60-year-old stand to 537 in the oldest forests. The 80-year-old stand showed the highest species richness and diversity values. With respect to species composition, large species such as <i>Carabus scheidleri</i> and <i>Carabus coriaceus</i> were dominant only in the oldest forests. Furthermore, species that overwinter in the larval stage were more abundant in the oldest forests (45% of the total number of individuals from the 150-year-old stand) than in the younger ones (20% of individuals from 60-year-old, and 22% of individuals from 80-year-old stands). Our results showed that the analyses of species composition and life history traits are valuable for estimating the conservation values of older forests. Although the investigated sites form part of a continuous forested area and are only a couple of kilometres apart, MIB values detect significant differences associated with forest age and can be a useful tool in evaluating the degree to which a forest reflects a natural state.",
					"doi": "10.3897/zookeys.100.1536",
					"journal": {
						"issue": "",
						"pages": "393-405",
						"title": "ZooKeys",
						"volume": "100"
					},
					"keywords": [
						"carabid beetles",
						"MIB",
						"over-wintering stages",
						"beech forests succession",
						"Papuk Nature Park"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2011-05-20",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "576847"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "782476"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Carabid beetle diversity and mean individual biomass in beech forests of various ages"
				},
				"owners": [
					1161
				],
				"revision": 7,
				"stats": {
					"downloads": 5,
					"unique_downloads": 5,
					"unique_views": 6,
					"version_downloads": 5,
					"version_unique_downloads": 5,
					"version_unique_views": 6,
					"version_views": 6,
					"version_volume": 4931650,
					"views": 6,
					"volume": 4931650
				},
				"updated": "2020-01-20T12:06:49.662710+00:00"
			},
			{
				"conceptrecid": "3366426",
				"created": "2019-08-13T04:30:43.854849+00:00",
				"doi": "10.3897/aca.2.e38819",
				"files": [
					{
						"bucket": "1a8a0008-f06b-4073-ae9f-f97ab0353e0b",
						"checksum": "md5:d46ee13baa315945ae763f9f2dcdc4b7",
						"key": "ACA_article_38819.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/1a8a0008-f06b-4073-ae9f-f97ab0353e0b/ACA_article_38819.pdf"
						},
						"size": 72643,
						"type": "pdf"
					},
					{
						"bucket": "1a8a0008-f06b-4073-ae9f-f97ab0353e0b",
						"checksum": "md5:b1689836512dc522780f12a199dd5b1f",
						"key": "ACA_article_38819.xml",
						"links": {
							"self": "https://zenodo.org/api/files/1a8a0008-f06b-4073-ae9f-f97ab0353e0b/ACA_article_38819.xml"
						},
						"size": 14325,
						"type": "xml"
					}
				],
				"id": 3366427,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e38819.svg",
					"bucket": "https://zenodo.org/api/files/1a8a0008-f06b-4073-ae9f-f97ab0353e0b",
					"doi": "https://doi.org/10.3897/aca.2.e38819",
					"html": "https://zenodo.org/record/3366427",
					"latest": "https://zenodo.org/api/records/3366427",
					"latest_html": "https://zenodo.org/record/3366427",
					"self": "https://zenodo.org/api/records/3366427"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Leuphana University Lüneburg, Lüneburg, Germany",
							"name": "Assmann, Thorsten"
						},
						{
							"affiliation": "Leuphana University Lüneburg, Lüneburg, Germany",
							"name": "Boutaud, Estève"
						},
						{
							"affiliation": "Ecosystem Monitoring, Research and Wildlife Conservation (SB 23 Invertebrates and Biodiversity), Black Forest National Park, Freudenstadt, Germany",
							"name": "Buse, Jörn"
						},
						{
							"affiliation": "Institute of Zoology, Hamburg, Germany",
							"name": "Drees, Claudia"
						},
						{
							"affiliation": "Tel Aviv University, Tel Aviv, Israel",
							"name": "Friedman, Ariel-Leib-Leonid"
						},
						{
							"affiliation": "Department of Biology and Biotechnology, American University of Madaba, Madaba, Jordan",
							"name": "Khoury, Fares"
						},
						{
							"affiliation": "Steinhardt Museum of Natural History, Tel Aviv University, Tel Aviv, Israel",
							"name": "Renan, Ittai"
						},
						{
							"affiliation": "Institute of Ecology, Leuphana University Lüneburg, Lüneburg, Germany",
							"name": "Schild, Laura"
						},
						{
							"affiliation": "Conservation Genetics Group, Senckenberg Research Institute, Research Station Gelnhausen , Gelnhausen, Germany",
							"name": "von Thaden, Alina"
						},
						{
							"affiliation": "ZHAW Zürcher Hochschule für Angewandte Wissenschaften, Wädenswil, Switzerland",
							"name": "Szallies, Alexander"
						},
						{
							"affiliation": "Leuphana University Lüneburg, Lüneburg, Germany",
							"name": "Zumstein, Pascale"
						}
					],
					"description": "<p>\n    In the face of the decline of many insects, there is an increasing demand for contemporary, fast and cost-effective approaches to monitor the development of populations and species. Numerous scientists favor molecular methods, especially those involving barcoding of the CO1 gene, as an alternative to classical, morphology-based species identification. Moreover, DNA barcoding is also discussed as a suitable method to support species delimitations in complexes of closely related taxa. We used the available sequences of ground beetles from North and Central Europe  with additional ones we generated from Southern Europe and the Middle East to draw conclusion about the practicability of such approach for ground beetles. \n  </p>\n  <p>\n    In general, while strong intraspecific differentiations within the CO1 fragment seem to characterize some wingless species (e.g. <em>Graphipterus serrator</em>, <em>Siagona longula</em>, <em>Carabus</em> <em>problematicus</em>, some <em>Platycarabus</em> species), others do not display much intraspecific variability (e.g. <em>Graphipterus multiguttatus</em> and <em>G. sharonae</em> within the \"<em>G. serrator </em>clade\"). These results certainly complicate the application of a metabarcoding approach without a larger database to delimitate these ground beetles. Furthermore, these results limit the applicability of the well-known barcoding gap, in ecological studies. \n  </p>\n  <p>\n    With regards to taxonomic problems, mitochondrial and nuclear DNA sequences can provide support for taxonomic decisions. For example, the two taxa <em>Carabus variolosus</em> and <em>nodulosus</em> are characterized predominantely by K2P values lower than the barcoding gap. In view of the otherwise strong intraspecific differentiation within the genus <em>Carabus</em>, these two taxa should be regarded as subspecies. In contrast, DNA barcoding can also help to identify \"good\" species. Mitochondrial and nuclear data suggest, for example, that an <em>Oreonebria</em> taxon and a <em>Platycarabus</em> taxon from the South-western Alps represent \"good species\", although they were usually considered as synonyms or subspecies. In another case, two tiger beetle taxa, which until a few months ago were considered to belong to the same species, show such strong differentiation that only two species can be postulated (<em>Calomera aulicoides</em> and <em>C. littoralis winkleri</em>). \n  </p>\n  <p>\n    In summary, we can state that DNA sequences and the barcoding gap can help to define species delimitations in ground beetles. However, several species, including widespread sister species, cannot be identified by DNA barcoding for various reasons (e.g. young species or horizontal gene flow). Consequently, until an automated, fast, and reliable method to identify species from samples emerges, ecological investigations have to rely on classical, morphology-based identifications. \n  </p>\n  <p></p>",
					"doi": "10.3897/aca.2.e38819",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e38819",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"DNA barcoding",
						"metabarcoding",
						"species identification",
						"species delineation",
						"species delimitation",
						"taxa",
						"automated species identification",
						"barcoding gap",
						"molecular taxonomy",
						"Carabidae",
						"Graphipterus",
						"Calomera",
						"Carabus",
						"Platycarabus",
						"Oreonebria",
						"Cicindela"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-08-05",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3366427"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3366426"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Heaven and hell: Spotlights on some DNA barcodes for species identification and delimitation in ground beetles"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 5,
					"unique_downloads": 2,
					"unique_views": 3,
					"version_downloads": 5,
					"version_unique_downloads": 2,
					"version_unique_views": 3,
					"version_views": 3,
					"version_volume": 246579,
					"views": 3,
					"volume": 246579
				},
				"updated": "2020-01-20T16:45:17.339090+00:00"
			},
			{
				"conceptdoi": "10.5281/zenodo.3336071",
				"conceptrecid": "3336071",
				"created": "2019-07-15T11:49:56.551179+00:00",
				"doi": "10.5281/zenodo.3336072",
				"files": [
					{
						"bucket": "974af387-2bb5-40b9-ba51-8eaeada37f53",
						"checksum": "md5:403f31be4ba20472c7c61993048e4970",
						"key": "Przyroda_25(online002).pdf",
						"links": {
							"self": "https://zenodo.org/api/files/974af387-2bb5-40b9-ba51-8eaeada37f53/Przyroda_25%28online002%29.pdf"
						},
						"size": 1250848,
						"type": "pdf"
					}
				],
				"id": 3336072,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.5281/zenodo.3336072.svg",
					"bucket": "https://zenodo.org/api/files/974af387-2bb5-40b9-ba51-8eaeada37f53",
					"conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.3336071.svg",
					"conceptdoi": "https://doi.org/10.5281/zenodo.3336071",
					"doi": "https://doi.org/10.5281/zenodo.3336072",
					"html": "https://zenodo.org/record/3336072",
					"latest": "https://zenodo.org/api/records/3336072",
					"latest_html": "https://zenodo.org/record/3336072",
					"self": "https://zenodo.org/api/records/3336072"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Katedra Zoologii, Wydział Biologii i Ochrony Środowiska, Uniwersytet Śląski w Katowicach, ul. Bankowa 9, 40-007 Katowice, Poland, artur.taszakowski@us.edu.pl",
							"name": "Artur Taszakowski",
							"orcid": "0000-0002-0885-353X"
						},
						{
							"affiliation": "Katedra Zoologii, Wydział Biologii i Ochrony Środowiska, Uniwersytet Śląski w Katowicach, ul. Bankowa 9, 40-007 Katowice, Poland, Studenckie Koło Naukowe Zoologów \"Faunatycy\", amaslowski@us.edu.pl,",
							"name": "Adrian Masłowski"
						},
						{
							"affiliation": "Muzeum i Instytut Zoologii Polskiej Akademii Nauk, ul. Wilcza 64, 00-679 Warszawa, Poland, lkarpinski@miiz.waw.pl,",
							"name": "Lech Karpiński",
							"orcid": "0000-0002-5475-3732"
						},
						{
							"affiliation": "Katedra Zoologii, Wydział Biologii i Ochrony Środowiska, Uniwersytet Śląski w Katowicach, ul. Bankowa 9, 40-007 Katowice, Poland, szczepanski.w@interia.pl",
							"name": "Wojciech T. Szczepański",
							"orcid": "0000-0003-0858-519X"
						},
						{
							"affiliation": "Park 9, 42-690 Brynek, Poland, henryk.szoltys@wp.pl",
							"name": "Henryk Szołtys"
						}
					],
					"description": "<p><strong>Materials to the knowledge of ground beetles (Coleoptera: Carabidae) of the Eastern Beskid Mountains</strong>. The paper presents new data on distribution of the family Carabidae. The study were carried out between 2001&ndash;2016 in south-western part of the Eastern Beskid Mountains. The list of 118 species of ground beetles is presented, including some taxa which are rarely collected in Poland. Four species:<em> Demetrias atricapillus </em>(Linnaeus, 1758), <em>Pterostichus quadrifoveolatus </em>Letzner, 1852, <em>Pterostichus rhaeticus </em>Heer, 1837 and <em>Tachyura diabrachys</em> (Kolenati, 1845) are recorded in this zoogeographical region for the first time. Moreover, the observation of representatives of horsehair worms Nematomorpha (especially of the genus <em>Gordionus</em> M&uuml;ller, 1927) which infected the specimen of <em>Carabus coriaceus</em> Linnaeus, 1758 is also mentioned.</p>",
					"doi": "10.5281/zenodo.3336072",
					"journal": {
						"issue": "online002",
						"pages": "1-18",
						"title": "ROCZNIK MUZEUM GÓRNOŚLĄSKIEGO W BYTOMIU, PRZYRODA",
						"volume": "25"
					},
					"keywords": [
						"biodiversity, Eastern Beskid Mountains, faunistics, ground beetles, Nematomorpha, Poland"
					],
					"language": "pol",
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-07-15",
					"references": [
						"Aleksandrowicz O. 2004. Wykaz gatunków – Coleoptera: Carabidae, pp. 32–42, In: Bogdanowicz W., Chudzicka E., Pilipiuk I., Skibińska E. (Eds), Fauna Polski – charakterystyka i wykaz gatunków. MiIZ PAN, Warszawa.",
						"Aleksandrowicz O. 2012. New record of Tachyura parvula (Dejean, 1831) (Coleoptera, Carabidae) from middle Pomerania Baltic Sea coast (N Poland). Baltic Coastal Zone. Journal of Ecology and Protection of the Coastline 16: 47–149.",
						"Burakowski B., Mroczkowski M., Stefańska J. 1973. Chrząszcze Coleoptera. Biegaczowate – Carabidae, cz. 1. Katalog fauny Polski 23(2): 1–232",
						"Burakowski B., Mroczkowski M., Stefańska J. 1974. Chrząszcze Coleoptera. Biegaczowate – Carabidae, cz. 2. Katalog fauny Polski 23(3): 1–430.",
						"Burakowski B., Mroczkowski M., Stefańska J. 2000. Chrząszcze, Coleoptera, Uzupełnienia tomów 2–21. Katalog Fauny Polski 23(22): 1–252.",
						"Gil R., Melke A. 2017. Owady z rzędu Coleoptera na terenie projektowanego Parku Krajobrazowego Beskidu Niskiego, In: Park Krajobrazowy \"Beskidu Niskiego\" Dokumentacja projektowa, Fundacja Dziedzictwo Przyrodnicze: 168–191.",
						"Jaskuła R., Kalisiak J., Szczepko K. 2003. Nowe stanowiska kilku rzadkich gatunków biegaczowatych (Coleoptera: Carabidae) w Polsce. Parki Narodowe i Rezerwaty Przyrody 22(2) 279–283.",
						"Jędryczkowski W.B., Kupryjanowicz J. 2005. Biegaczowate, Carabidae (chrząszcze, Coleoptera) czterech Środowisk Biebrzańskiego Parku Narodowego, In: Dyrcz A., Werpachowski C, Przyroda Biebrzańskiego Parku Narodowego. Biebrzański Park Narodowy, Osowiec-Twierdza: 325–329",
						"Karpiński L., Taszakowski A., Szczepański W.T. 2015. New data on the occurrence of longhorn beetles (Coleoptera: Cerambycidae) in the Eastern Beskid Mountains. Fragmenta Faunistica 58(1): 7–16.",
						"Kaszyca N., Taszakowski A. 2017. Materiały do znajomości chrząszczy z nadrodziny Scarabaeoidea Beskidu Wschodniego. Acta entomologica silesiana 25(013): 117–123",
						"Knutelski S., Tykarski P. 2010. Chrząszcze obszarów górskich Polski (Insecta: Coleoptera). Wiadomości Entomologiczne 29(Supl.): 39–52.",
						"Kondracki J. 2013. Geografia regionalna Polski. Wydawnictwo Naukowe PWN, Warszawa: 440 pp.",
						"Konopko D., Wilga M.S. 2014. Przyczynek do poznania chrząszczy Coleoptera Trójmiejskiego Parku Krajobrazowego. Przegląd Przyrodniczy 25(1): 64–71.",
						"Konwerski S., Sienkiewicz P. 2002. Przyczynek do poznania chrząszczy Beskidu Niskiego. Nowy Pamiętnik Fizjograficzny 1(1): 85–88.",
						"Kopecky T. 2003. Subtribe Tachyina Motschulsky, 1862, pp. 273–280, In: Löebl I., Smetana A. (Eds.), Catalogue of Palaearctic Coleoptera. Vol. 1. Archostemata-Myxophaga-Adephaga. Apollo Books, Stenstrup.",
						"Kosewska A., Nietupski M., Ciepielewska D. 2006. Skład i struktura zgrupowań Carabidae (Coleoptera) zasiedlających zadrzewienia śródpolne okolic Olsztyna, In: Biegaczowate (Coleoptera: Carabidae) środowisk antropogenicznych. Wiadomości Entomologiczne 25(Supl. 1): 49–59.",
						"Löbl I., Smetana A. 2003. Catalogue of Palaearctic Coleoptera. Vol. 1. Archostemata-Myxophaga-Adephaga. Apollo Books, Stenstrup, 819 pp.",
						"Mapy klimatu Polski. Dostęp 14.03.2018. http://klimat.pogodynka.pl/pl/climate-maps.",
						"Pawłowski J. 1974. Chrząszcze – Coleoptera, Biegaczowate – Carabidae. Podrodziny Bembidinae, Trechinae. Klucze do Oznaczania Owadów Polski 19(3b): 1– 94.",
						"Pawłowski J. 2009. Cenne bezkręgowce naziemne Magurskiego Parku Narodowego i terenów ościennych, pp. 132–146, In: Górecki A., Zemanek B. (Eds.), Magurski Park Narodowy – monografia przyrodnicza, Krempna-Kraków.",
						"Pilipiuk I. 2008. Nitnikowce, drucieńce (Nematomorpha), pp. 479–480, In: Bogdanowicz W., Chudzicka E., Pilipiuk I., Skibińska E. (Eds.), Fauna Polski – charakterystyka i wykaz gatunków. T. III. MiIZ PAN, Warszawa.",
						"Sienkiewicz P., Konwerski S., Przewoźny M. 2009. Nowe dane o występowaniu chrząszczy (Coleoptera) z wybranych rodzin na terenie Rogalińskiego Parku Krajobrazowego. Cz. I. Biegaczowate (Carabidae). Wiadomości Entomologiczne 28(4): 219–230.",
						"Szczepański W.T., Karpiński L., Taszkowski A. 2013. Nowe stanowiska Omalisus (Omalisus) fontisbellaquaei Geoffroy, 1785 (Coleoptera: Omalisidae) w południowej Polsce. Acta entomologica silesiana 21: 73.",
						"Szczepański W.T., Taszakowski A., Karpiński L. 2014. Nowe stanowisko Hemicoelus costatus (Aragona, 1830) (Coleoptera: Ptinidae) w Polsce. Acta entomologica silesiana 22: 55.",
						"Szczepański W.T., Taszakowski A., Karpiński L. 2015a. Nowe stanowiska bogatkowatych (Buprestidae) w Beskidzie Wschodnim. Acta entomologica silesiana 23(030): 205–208.",
						"Szczepański W.T., Taszakowski A., Karpiński L. 2015b. Nowe stanowiska Cassida panzeri Weise, 1907 (Coleoptera: Chrysomelidae) w południowej Polsce. Acta entomologica silesiana 23(023): 227.",
						"Szczepański W.T., Taszakowski A., Karpiński L., Kubusiak A. 2015c. New data on the distribution of ladybird beetles (Coleoptera: Coccinellidae) of the Eastern Beskid Mts. Nature Journal (Opole Scientific Society) 48: 24–33.",
						"Szczepański W.T., Taszakowski A., Karpiński L., Morawski M. 2015d. Nowe stanowiska biegaczowatych (Coleoptera: Carabidae) w Beskidzie Wschodnim. IV Ogólnopolska Konferencja Młodych Naukowców \"Arthropod\", 28-31 czerwiec 2015, Uniwersytet Śląski w Katowicach.",
						"Szczepański W.T., Taszakowski A., Karpiński L., Tomecka M. 2015e. Materiały do znajomości omomiłkowatych, karmazynkowatych i świetlikowatych (Coleoptera: Elateroidea: Cantharidae, Lycidae, Lampyridae) Beskidu Wschodniego. Acta entomologica silesiana 23(003): 7–13.",
						"Szczepański W.T., Taszakowski A., Karpiński L., Kaszyca N. 2016. Nowe stanowiska sprężykowatych (Coleoptera: Elateridae) w Beskidzie Wschodnim. Acta entomologica silesiana 24(001): 7–15.",
						"Szołtys H., Taszakowski A. 2017. Isorhipis nigriceps (Mannerheim, 1823) – nowy dla fauny Polski gatunek chrząszcza (Coleoptera: Eucnemidae). Acta entomologica silesiana 25(031): 161–165.",
						"Taszakowski A. 2012. Występowanie Eysarcoris ventralis (Westwood, 1837) (Hemiptera: Pentatomidae) w Polsce. Acta entomologica silesiana 20: 33–55.",
						"Taszakowski A. 2016. Brudząca oczyszczalnia, In: Bonk M, Małe rzeki – blog przyrodniczy. Dostęp 14.03.2018. https://malerzeki.wordpress.com.",
						"Taszakowski A., Baran B., Kaszyca N,. Depa Ł. 2015. Genus Claviger Preyssler, 1790 (Coleoptera: Staphylinidae: Pselaphinae) in the Low Beskid Mts. (Poland) – new sites and host affiliation. Nature Journal (Opole Scientific Society) 48: 114–119.",
						"Taszakowski A., Kolak G. 2015. Drugie stwierdzenie Oxycarenus pallens (Herrich-Schaeffer, 1850) (Hemiptera: Heteroptera: Oxycarenidae) na terenie Polski. Heteroptera Poloniae – Acta Faunistica 9: 7–8.",
						"Taszakowski A., Kaszyca N., Mazur M.A. 2017. Materiały do znajomości ryjkowców (Coleoptera: Curculionoidea) Beskidu Wschodniego. Acta entomologica silesiana 25(006): 71–88.",
						"Taszakowski A., Kaszyca N., Szołtys H. 2018. Materiały do znajomości Staphyliniformia (Coleoptera) Beskidu Wschodniego. Acta entomologica silesiana 26(003): 35–44. DOI: 10.5281/zenodo.1175615.",
						"Taszakowski A., Morawski M., Szołtys H., Szczepański W.T. 2017. Materiały do znajomości stonkowatych (Coleoptera: Chrysomelidae) Beskidu Wschodniego. Rocznik Muzeum Górnośląskiego w Bytomiu, Przyroda 23(004): 55–71. DOI: 10.5281/zenodo.1065932.",
						"Taszakowski A., Szczepański W.T., Baran B., Morawski M. 2014. Nowe stanowiska Oxythyrea funesta (Poda, 1761) (Coleoptera: Scarabeidae) w Polsce. Acta entomologica silesiana 22: 56–57.",
						"Thomas M.B., Sotherton N.W., Coombes D.S., Wratten S.D. 1992. Habitat factors influencing the distribution of polyphagous predatory insects between field boundaries. Annals of Applied Biology 120: 197–202.",
						"Wojas T. 1992. Nowe stanowiska kilku rzadkich gatunków biegaczowatych (Coleoptera, Carabidae) w Polsce. Wiadomości entomologiczne 11(3): 143–147.",
						"Wojas T. 2008. Biegaczowate (Coleoptera, Carabidae) Gorców. Ochrona Beskidów Zachodnich 2: 51–101."
					],
					"related_identifiers": [
						{
							"identifier": "10.5281/zenodo.3336071",
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
									"pid_value": "3336072"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3336071"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Materiały do znajomości biegaczowatych (Coleoptera: Carabidae) Beskidu Wschodniego"
				},
				"owners": [
					30145
				],
				"revision": 4,
				"stats": {
					"downloads": 19,
					"unique_downloads": 19,
					"unique_views": 15,
					"version_downloads": 19,
					"version_unique_downloads": 19,
					"version_unique_views": 15,
					"version_views": 15,
					"version_volume": 23766112,
					"views": 15,
					"volume": 23766112
				},
				"updated": "2020-01-20T14:19:13.898621+00:00"
			},
			{
				"conceptrecid": "636734",
				"created": "2016-06-15T17:33:37+00:00",
				"doi": "10.3897/BDJ.4.e8135",
				"files": [
					{
						"bucket": "e4459c18-4e70-43df-a219-e47e3811ff45",
						"checksum": "md5:3795792a987dcf67e4267458b92d84a5",
						"key": "BDJ_article_8135.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/e4459c18-4e70-43df-a219-e47e3811ff45/BDJ_article_8135.pdf"
						},
						"size": 721910,
						"type": "pdf"
					},
					{
						"bucket": "e4459c18-4e70-43df-a219-e47e3811ff45",
						"checksum": "md5:ac52602206418313a9a12847347c8383",
						"key": "BDJ_article_8135.xml",
						"links": {
							"self": "https://zenodo.org/api/files/e4459c18-4e70-43df-a219-e47e3811ff45/BDJ_article_8135.xml"
						},
						"size": 2021792,
						"type": "xml"
					}
				],
				"id": 54955,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/BDJ.4.e8135.svg",
					"bucket": "https://zenodo.org/api/files/e4459c18-4e70-43df-a219-e47e3811ff45",
					"doi": "https://doi.org/10.3897/BDJ.4.e8135",
					"html": "https://zenodo.org/record/54955",
					"latest": "https://zenodo.org/api/records/54955",
					"latest_html": "https://zenodo.org/record/54955",
					"self": "https://zenodo.org/api/records/54955"
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
							"affiliation": "Sofia University, Faculty of Biology, Sofia, Bulgaria",
							"name": "Kostova, Rumyana"
						},
						{
							"affiliation": "National Museum of Natural History Sofia, Sofia, Bulgaria",
							"name": "Guéorguiev, Borislav"
						}
					],
					"description": "<p>The knowledge of the ground-beetle fauna of Strandzha is currently incomplete, and is largely based on data from the Bulgarian part of the region and on records resulting from casual collecting. This study represents a critical revision of the available literature, museum collections and a three years field study of the carabid beetles of the Bulgarian and Turkish parts of Strandzha Mountain and the adjacent Black Sea Coast territories.</p>\n<p>A total of 328 species and subspecies of Carabidae, belonging to 327 species from the region of Strandzha Mountain and adjacent seacoast area, have been listed. Of these, 77 taxa represent new records for the Bulgarian part of the region, and 110 taxa new records for Turkish part of the studied region.</p>\n<p>Two taxa, one subgenus (<i>Haptotapinus</i> Reitter, 1886) and one species (<i>Pterostichus crassiusculus</i>), are new to the fauna of Bulgaria. Based on a misidentification, the species <i>Apotomus testaceus</i> is excluded from the list of the Bulgarian fauna. Seven species (<i>Carabus violaceus azurescens</i>, <i>Apotomus rufus</i>, <i>Platynus proximus</i>, <i>Molops alpestris kalofericus</i>, <i>M. dilatatus angulicollis</i>, <i>Pterostichus merklii</i>, and <i>Calathus metallicus</i>) are treated as doubtful for the regional fauna, and one (<i>Apotomus rufus</i>) also for the Bulgarian fauna.</p>\n<p>Altogether, 43 taxa collected in the Turkish part of the region are new for European Turkey. New taxa for Turkey are the genera <i>Myas</i> and <i>Oxypselaphus</i>, the subgenus <i>Feronidius</i>, and nine species and subspecies (<i>Carabus granulatus granulatus</i>, <i>Dyschirius tristis</i>, <i>Bembidion normannum apfelbecki</i>, <i>B. subcostatum vau</i>, <i>Acupalpus exiguus</i>, <i>Myas chalybaeus</i>, <i>Oxypselaphus obscurus</i>, <i>Pterostichus leonisi</i>, <i>Pt. melas</i>). In addition, there are a further seven species that are here confirmed for Turkey.</p>",
					"doi": "10.3897/BDJ.4.e8135",
					"journal": {
						"issue": "",
						"pages": "e8135",
						"title": "Biodiversity Data Journal",
						"volume": "4"
					},
					"keywords": [
						"Animalia",
						"Arthropoda",
						"Insecta",
						"ColeopteraAnimalia",
						"Coleoptera",
						"Caraboidea",
						"Carabidae",
						"Carabidae",
						"Strandzha",
						"Yildiz",
						"Bulgaria",
						"European part of Turkey"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2016-04-01",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "54955"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "636734"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "The ground beetles (Coleoptera: Carabidae) of the Strandzha Mountain and adjacent coastal territories (Bulgaria and Turkey)"
				},
				"owners": [
					1161
				],
				"revision": 13,
				"stats": {
					"downloads": 27,
					"unique_downloads": 26,
					"unique_views": 7,
					"version_downloads": 27,
					"version_unique_downloads": 26,
					"version_unique_views": 7,
					"version_views": 7,
					"version_volume": 19491570,
					"views": 7,
					"volume": 19491570
				},
				"updated": "2020-01-20T14:48:12.860766+00:00"
			},
			{
				"conceptrecid": "783026",
				"created": "2017-05-12T15:23:19.680927+00:00",
				"doi": "10.3897/zookeys.147.2097",
				"files": [
					{
						"bucket": "d90d78af-a28c-40e4-8f3d-18428cd409bb",
						"checksum": "md5:85d42f304c011c44826314ffaaa182e1",
						"key": "ZK_article_2940.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/d90d78af-a28c-40e4-8f3d-18428cd409bb/ZK_article_2940.pdf"
						},
						"size": 2106863,
						"type": "pdf"
					},
					{
						"bucket": "d90d78af-a28c-40e4-8f3d-18428cd409bb",
						"checksum": "md5:39a6d9596183711811134477aca32aed",
						"key": "ZK_article_2940.xml",
						"links": {
							"self": "https://zenodo.org/api/files/d90d78af-a28c-40e4-8f3d-18428cd409bb/ZK_article_2940.xml"
						},
						"size": 59530,
						"type": "xml"
					}
				],
				"id": 577397,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.147.2097.svg",
					"bucket": "https://zenodo.org/api/files/d90d78af-a28c-40e4-8f3d-18428cd409bb",
					"doi": "https://doi.org/10.3897/zookeys.147.2097",
					"html": "https://zenodo.org/record/577397",
					"latest": "https://zenodo.org/api/records/577397",
					"latest_html": "https://zenodo.org/record/577397",
					"self": "https://zenodo.org/api/records/577397"
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
							"affiliation": "University of Alberta, Edmonton, Canada",
							"name": "Bourassa, Stephane"
						},
						{
							"affiliation": ", , Canada",
							"name": "Spence, John"
						},
						{
							"affiliation": "University of Alberta, Edmonton, Canada",
							"name": "Hartley, Dustin J."
						},
						{
							"affiliation": "University of Alberta, Edmonton, Canada",
							"name": "Lee, Seung Il"
						}
					],
					"description": "<p>A study spanning ten years revealed changes in wing-morph ratios corroborating the hypothesis that the wing-dimorphic introduced carabid, <i>Pterostichus melanarius </i>Ill.,<i> </i>is spreading through flight, from the city of Edmonton, Canada and establishing populations in natural aspen forest of more rural areas 45-50 km to the East. Comparison of wing-morph ratios between <i>P. melanarius</i> and the native wing dimorphic species <i>Agonum retractum</i> LeConte suggests that the spatial variation in ratios for <i>P. melanarius</i> does not reflect underlying environmental variation, but instead the action of selective forces on this wing-dimorphic species. About ten years after its earliest detection in some rural sites the frequency of macropterous individuals in <i>P. melanarius</i> has decreased <i>c.</i> five-fold, but it is still above the level seen in European populations in which the two wing-morphs are thought to exist in equilibrium. <i>P. melanarius</i> is expanding its range in native aspen forest much faster than three other introduced species <i>Clivina fossor </i>L.), <i>Carabus granulatus </i>O.F. Müller<i> </i>and <i>Clivina fossor </i>L also encountered in this study. The two <i>Carabus </i>species are flightless, but <i>C. fossor</i> can be dimorphic. Although these four non-native ground beetle species comprise &gt;85% of the carabids collected at sites in urban Edmonton, activity-density of native carabids was similar across the urban-rural gradient, suggesting little direct impact of introduced species on the local abundance of native species. In a second study conducted at a smaller scale near George Lake, Alberta, macropterous individuals of <i>P. melanarius</i> have penetrated furthest and most rapidly into native aspen forest. Furthermore, the percentage of micropterous individuals has increased markedly in areas first colonized a decade previously. Overall, these studies support the idea that macropterous beetles in wing-d dimorphic species are important vanguards for early colonization of unexploited territory, but that flightless individuals replace the flying morph relatively rapidly once populations are established.</p>",
					"doi": "10.3897/zookeys.147.2097",
					"journal": {
						"issue": "",
						"pages": "545-558",
						"title": "ZooKeys",
						"volume": "147"
					},
					"keywords": [
						"Pterostichus melanarius",
						"wing-dimorphism"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2011-11-16",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "577397"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "783026"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Wing-dimorphism and population expansion of Pterostichus melanarius (Illiger, 1798) at small and large scales in central Alberta, Canada (Coleoptera, Carabidae, Pterostichini)"
				},
				"owners": [
					1161
				],
				"revision": 8,
				"stats": {
					"downloads": 21,
					"unique_downloads": 21,
					"unique_views": 12,
					"version_downloads": 21,
					"version_unique_downloads": 21,
					"version_unique_views": 12,
					"version_views": 13,
					"version_volume": 44244123,
					"views": 13,
					"volume": 44244123
				},
				"updated": "2020-01-20T15:20:21.304976+00:00"
			},
			{
				"conceptdoi": "10.5281/zenodo.3665226",
				"conceptrecid": "3665226",
				"created": "2020-02-12T13:51:47.157961+00:00",
				"doi": "10.5281/zenodo.3665227",
				"files": [
					{
						"bucket": "327b344b-2cc1-4dff-b621-106561ea7aae",
						"checksum": "md5:ff29f94cf386fa8eaf234a9c69a1aa49",
						"key": "treatment.html",
						"links": {
							"self": "https://zenodo.org/api/files/327b344b-2cc1-4dff-b621-106561ea7aae/treatment.html"
						},
						"size": 3580,
						"type": "html"
					}
				],
				"id": 3665227,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.5281/zenodo.3665227.svg",
					"bucket": "https://zenodo.org/api/files/327b344b-2cc1-4dff-b621-106561ea7aae",
					"conceptbadge": "https://zenodo.org/badge/doi/10.5281/zenodo.3665226.svg",
					"conceptdoi": "https://doi.org/10.5281/zenodo.3665226",
					"doi": "https://doi.org/10.5281/zenodo.3665227",
					"html": "https://zenodo.org/record/3665227",
					"latest": "https://zenodo.org/api/records/3665227",
					"latest_html": "https://zenodo.org/record/3665227",
					"self": "https://zenodo.org/api/records/3665227"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"alternate_identifiers": [
						{
							"identifier": "http://treatment.plazi.org/id/03D77E1287136B1CFF0EFC7D656EFEDD",
							"scheme": "url"
						}
					],
					"communities": [
						{
							"id": "biosyslit"
						}
					],
					"creators": [
						{
							"name": "Sciaky, Riccardo"
						},
						{
							"name": "Anichtchenko, Alexander"
						}
					],
					"custom": {
						"dwc:family": [
							"Carabidae"
						],
						"dwc:genus": [
							"Drypta"
						],
						"dwc:kingdom": [
							"Animalia"
						],
						"dwc:order": [
							"Coleoptera"
						],
						"dwc:phylum": [
							"Arthropoda"
						],
						"dwc:scientificNameAuthorship": [
							"Latreille"
						],
						"dwc:taxonRank": [
							"genus"
						],
						"openbiodiv:TaxonomicConceptLabel": [
							"Drypta Latreille, 1796 sec. Sciaky & Anichtchenko, 2020"
						]
					},
					"description": "<i> Drypta</i> Latreille, 1796<p> Type species:<i> Carabus emarginatus</i> Gmelin, 1790 (=<i> Carabus dentatus</i> P. Rossi, 1790)</p><p> =<i> Desera</i> Dejean, 1825 (nec Hope, 1831) Type species:<i> Drypta longicollis</i> MacLeay, 1835</p><p> =<i> Deserida</i> Basilewsky, 1960 Type species:<i> Carabus distinctus</i> P. Rossi, 1792</p><p> =<i> Dryptella</i> Jeannel, 1949 Type species:<i> Drypta cyanella</i> Chaudoir, 1843</p><p> This is the nominotypical genus of the tribe; it contains around 47 species diffused in Africa, Asia, Australia and, very marginally, in Europe.</p><p> Liang et al. (2004) have correctly pointed out the reasons for which<i> Desera</i> must be regarded as a synonym of<i> Drypta</i> and its long-lasting confusion with<i> Dendrocellus</i>, due to the misinterpretation of<i> Drypta longicollis</i> MacLeay.</p><p><i> Deserida</i> was erected by Basilewsky (1960) as a substitution name for the species near<i> D. distincta</i>, since this author regarded<i> Desera</i> as the valid name for the genus presently called<i> Dendrocellus</i>. This generic (or subgeneric) epithet has been frequently used for the pale species of<i> Drypta</i>, in which the elytra instead of being metallic are yellowish with darker margins or completely brown. This taxon has already been considered as a synonym of<i> Drypta</i> by Habu (1967) and we completely agree with this point of view. In our opinion the characters that should allow separation of this taxon from<i> Drypta</i> are inconsistent: the apical margin of elytra obliquely truncate instead of perpendicular to the suture is a character at the same time very variable and difficult to appreciate. Beyond that, we could not find any other reliable differentiating character. Even the shape of the body, shorter and stouter according to Jeannel (1949), is almost identical for example in the type species of<i> Drypta</i> (<i> D. dentata</i>) and of<i> Deserida</i> (<i> D. distincta</i>), while other species belonging to both groups are much more slender and elongate.</p><p><i> Dryptella</i> is a subgenus described by Jeannel (1949) for the majority of the African species of<i> Drypta</i>, but also in this case the characters pointed out (shape more slender and elongate, occurrence of a carina on interval 9) are very doubtful and difficult to observe, sometimes almost illusionary, at least in our opinion widely insufficient for a subgeneric distinction.<i> Dryptella</i> has already been regarded as synonym of<i> Drypta</i> by Habu (1967) and we agree with this position.</p><p> The unique combination of characters distinguishing<i> Drypta</i> from the other genera of the tribe is: pronotal bead absent or rudimental (fig. 9); punctuation on head and pronotum dense, more or less regular, the punctures usually distinct from each other, not confluent; pronotum very feebly constricted towards base; elytral microsculpture well developed; elytral pubescence dense, usually arranged in two-three more or less regular rows; number of scutellar pores varied from 1 to 4, but most frequently 1; intervals flat or slightly convex; tarsal claws thick, strongly curved, and smooth on inner side; two or three evident setae on outer side of stylomere (fig. 7).</p>",
					"doi": "10.5281/zenodo.3665227",
					"journal": {
						"issue": "4",
						"pages": "523",
						"title": "Taxonomic notes on the tribe Dryptini Bonelli, 1810 with description of a new genus and species from China (Coleoptera: Carabidae: Dryptini), pp. 522-530 in Zootaxa",
						"volume": "4731"
					},
					"keywords": [
						"Biodiversity",
						"Taxonomy",
						"Animalia",
						"Arthropoda",
						"Insecta",
						"Coleoptera",
						"Carabidae",
						"Drypta"
					],
					"license": {
						"id": "notspecified"
					},
					"notes": "Published as part of <i>Sciaky, Riccardo &amp; Anichtchenko, Alexander, 2020, Taxonomic notes on the tribe Dryptini Bonelli, 1810 with description of a new genus and species from China (Coleoptera: Carabidae: Dryptini), pp. 522-530 in Zootaxa 4731 (4)</i> on page 523, DOI: 10.11646/zootaxa.4731.4.5, <a href=\"http://zenodo.org/record/3661980\">http://zenodo.org/record/3661980</a>",
					"publication_date": "2020-02-10",
					"references": [
						"Basilewsky, P. (1960) Etude des Dryptinae d'Afrique (Coleoptera, Carabidae). Bulletin & Annales de la Societe entomologique de Belgique, 96 (5 - 8), 133 - 182.",
						"Jeannel, R. (1949) Faune de l'empire francais. XI. Coleopteres carabiques de la region Malgache. Troisieme Partie. Libriarie Larose Paris, 380 pp. [pp. 767 - 1146]",
						"Liang, H., Kavanaugh, D. H. & Tian, M. (2004) Notes on Drypta longicollis MacLeay and the Status of the Genus-group Name Desera Dejean, 1825 (Coleoptera: Carabidae: Dryptini). Proceedings of the California Academy of Sciences, 55 (18), 377 - 383.",
						"Habu, A. (1967) Carabidae. Truncatipennes group. (Insecta: Coleoptera). Fauna Japonica. Tokyo Electrical Engineering College Press, Tokyo, 338 pp., 27 pls."
					],
					"related_identifiers": [
						{
							"identifier": "10.11646/zootaxa.4731.4.5",
							"relation": "isPartOf",
							"resource_type": "publication-article",
							"scheme": "doi"
						},
						{
							"identifier": "http://zenodo.org/record/3661980",
							"relation": "isPartOf",
							"resource_type": "publication-article",
							"scheme": "url"
						},
						{
							"identifier": "http://publication.plazi.org/id/FFEE066A87126B1EFF99FF946108FFC2",
							"relation": "isPartOf",
							"resource_type": "publication-article",
							"scheme": "url"
						},
						{
							"identifier": "http://zoobank.org/47B975A5-547D-470E-B94E-05B8128C1A69",
							"relation": "isPartOf",
							"resource_type": "publication-article",
							"scheme": "url"
						},
						{
							"identifier": "10.5281/zenodo.3665226",
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
									"pid_value": "3665227"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3665226"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "taxonomictreatment",
						"title": "Taxonomic treatment",
						"type": "publication"
					},
					"title": "Drypta Latreille 1796"
				},
				"owners": [
					1161
				],
				"revision": 2,
				"stats": {
					"downloads": 0,
					"unique_downloads": 0,
					"unique_views": 0,
					"version_downloads": 0,
					"version_unique_downloads": 0,
					"version_unique_views": 0,
					"version_views": 0,
					"version_volume": 0,
					"views": 0,
					"volume": 0
				},
				"updated": "2020-02-12T19:21:05.319949+00:00"
			},
			{
				"conceptrecid": "3352456",
				"created": "2019-07-27T04:31:12.722576+00:00",
				"doi": "10.3897/aca.2.e38376",
				"files": [
					{
						"bucket": "c6e9e03d-7170-4876-8e11-79b076435e57",
						"checksum": "md5:fa58250eceafb7be5b767c3fbeb98463",
						"key": "ACA_article_38376.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/c6e9e03d-7170-4876-8e11-79b076435e57/ACA_article_38376.pdf"
						},
						"size": 52650,
						"type": "pdf"
					},
					{
						"bucket": "c6e9e03d-7170-4876-8e11-79b076435e57",
						"checksum": "md5:07e1df243f08e0ed109008f3e6e71501",
						"key": "ACA_article_38376.xml",
						"links": {
							"self": "https://zenodo.org/api/files/c6e9e03d-7170-4876-8e11-79b076435e57/ACA_article_38376.xml"
						},
						"size": 6298,
						"type": "xml"
					}
				],
				"id": 3352457,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e38376.svg",
					"bucket": "https://zenodo.org/api/files/c6e9e03d-7170-4876-8e11-79b076435e57",
					"doi": "https://doi.org/10.3897/aca.2.e38376",
					"html": "https://zenodo.org/record/3352457",
					"latest": "https://zenodo.org/api/records/3352457",
					"latest_html": "https://zenodo.org/record/3352457",
					"self": "https://zenodo.org/api/records/3352457"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "Finnish Natural Resources Institute, Helsinki, Finland|University of Eastern Finland, Joensuu, Finland",
							"name": "Koivula, Matti"
						}
					],
					"description": "<p>Urban forests are regularly managed for human safety and aesthetic reasons, but they are crucial habitat for many species. Removals of undergrowth occur commonly in these forests, yet the ecological consequences of these operations are poorly understood. We sampled ground beetles (Coleoptera, Carabidae) along 20-m edge gradients in Finnish urban forests, in five stands treated 0.5−2.5 years earlier with undergrowth removal and in five untreated stands. We hypothesized that undergrowth removal and edge proximity would benefit opportunistic and open-habitat species, whereas shady-habitat species would be affected negatively.</p>\n              \n                Diversity and evenness indices, open-habitat species and Carabus nemoralis responded positively, and forest species, Leistus terminatus and Pterostichus oblongopunctatus responded negatively, to the undergrowth removal.\n                Edge proximity had little effect on carabids.\n              \n              <p>However, open-habitat carabids were less abundant and less speciose 10−20 m from than right at the edge. We conclude that, while managing urban forests, undergrowth removals should be avoided at sites that host rare or threatened forest-associated species.</p>",
					"doi": "10.3897/aca.2.e38376",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e38376",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"Carabidae",
						"edge effect",
						"forest management"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-07-19",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3352457"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3352456"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Effects of undergrowth removal and edge proximity on ground beetles in urban boreal forests"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 11,
					"unique_downloads": 8,
					"unique_views": 4,
					"version_downloads": 11,
					"version_unique_downloads": 8,
					"version_unique_views": 4,
					"version_views": 4,
					"version_volume": 486446,
					"views": 4,
					"volume": 486446
				},
				"updated": "2020-01-20T17:19:28.650831+00:00"
			},
			{
				"conceptrecid": "3361067",
				"created": "2019-08-06T04:31:46.744859+00:00",
				"doi": "10.3897/aca.2.e38519",
				"files": [
					{
						"bucket": "c2e24dee-32cb-4e1b-a7e5-d4b2625f291d",
						"checksum": "md5:497a380f1e56be91efe3c6bbe25720a1",
						"key": "ACA_article_38519.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/c2e24dee-32cb-4e1b-a7e5-d4b2625f291d/ACA_article_38519.pdf"
						},
						"size": 59535,
						"type": "pdf"
					},
					{
						"bucket": "c2e24dee-32cb-4e1b-a7e5-d4b2625f291d",
						"checksum": "md5:2a9e389aad1168f457fa2b554faf046b",
						"key": "ACA_article_38519.xml",
						"links": {
							"self": "https://zenodo.org/api/files/c2e24dee-32cb-4e1b-a7e5-d4b2625f291d/ACA_article_38519.xml"
						},
						"size": 6834,
						"type": "xml"
					}
				],
				"id": 3361068,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/aca.2.e38519.svg",
					"bucket": "https://zenodo.org/api/files/c2e24dee-32cb-4e1b-a7e5-d4b2625f291d",
					"doi": "https://doi.org/10.3897/aca.2.e38519",
					"html": "https://zenodo.org/record/3361068",
					"latest": "https://zenodo.org/api/records/3361068",
					"latest_html": "https://zenodo.org/record/3361068",
					"self": "https://zenodo.org/api/records/3361068"
				},
				"metadata": {
					"access_right": "open",
					"access_right_category": "success",
					"creators": [
						{
							"affiliation": "University of Alberta, Edmonton, Canada",
							"name": "Bergeron, Colin"
						},
						{
							"affiliation": "Université du Québec à Rimouski, Rimouski, Canada",
							"name": "Arseneault, Dominique"
						}
					],
					"description": "<p>Variation in fire severity strongly influences post-fire forest development. The resulting fine scale forest heterogeneity could impact biodiversity over long periods after fire events. In the James Bay area of northern Québec, differential seed mortality caused by high and low crown fire severity resulted in dramatic variation in regeneration density of both jack pine and black spruce. Sixty years after such fire event, we show that composition of lichen and carabid assemblages varied significantly between areas of high (c. 2600 stems/ha) and low (c. 560 stems/ha) stem density established by differential crown fire severity. The carabids, <em>Notiophilus semistriatus</em> and <em>Miscodera arctica,</em> were found in low stem density areas while <em>Carabus taedatus</em> and <em>Pterostichus brevicornis</em> were found in high stem density areas. Amount of bare ground was higher in low stem density area which may favor active visual diurnal hunters such as <em>Notiophilus</em> species. <em>Cladonia rangiferina</em> and <em>C. stellaris</em> were associated with high stem density area while <em>C. uncialis</em> and <em>C. mitis</em> were associated with low stem density area. This likely reflects the fact that photosynthetic rate of <em>C. rangiferina </em>is optimal under shady areas whereas <em>C. uncialis</em> is better adapted to hot, dry and sunny conditions. Thus, variation in fire behavior led to long-lasting variation in forest conditions that clearly affected both lichen and carabid assemblages even 60 years after fire.</p>",
					"doi": "10.3897/aca.2.e38519",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "e38519",
						"title": "ARPHA Conference Abstracts",
						"volume": "2"
					},
					"keywords": [
						"Fire behavior",
						"Fire severity",
						"carabidae",
						"lichens",
						"long-term effects",
						"post-fire regeneration"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2019-07-29",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "3361068"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "3361067"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Long term effect of fire severity on carabid and lichen assemblages"
				},
				"owners": [
					1161
				],
				"revision": 4,
				"stats": {
					"downloads": 10,
					"unique_downloads": 7,
					"unique_views": 6,
					"version_downloads": 10,
					"version_unique_downloads": 7,
					"version_unique_views": 6,
					"version_views": 6,
					"version_volume": 489948,
					"views": 6,
					"volume": 489948
				},
				"updated": "2020-01-20T17:00:19.069528+00:00"
			},
			{
				"conceptrecid": "1240602",
				"created": "2018-05-04T04:30:25.908712+00:00",
				"doi": "10.3897/zookeys.753.22366",
				"files": [
					{
						"bucket": "3c918d3c-339e-443e-939b-3fc24ecf38d2",
						"checksum": "md5:9b001609516ce3dadb60a6e438eca69a",
						"key": "ZK_article_22366.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/3c918d3c-339e-443e-939b-3fc24ecf38d2/ZK_article_22366.pdf"
						},
						"size": 25243549,
						"type": "pdf"
					},
					{
						"bucket": "3c918d3c-339e-443e-939b-3fc24ecf38d2",
						"checksum": "md5:4b39cb0d9b8183dcb9a63ef9da5cbbf5",
						"key": "ZK_article_22366.xml",
						"links": {
							"self": "https://zenodo.org/api/files/3c918d3c-339e-443e-939b-3fc24ecf38d2/ZK_article_22366.xml"
						},
						"size": 417288,
						"type": "xml"
					}
				],
				"id": 1240603,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.753.22366.svg",
					"bucket": "https://zenodo.org/api/files/3c918d3c-339e-443e-939b-3fc24ecf38d2",
					"doi": "https://doi.org/10.3897/zookeys.753.22366",
					"html": "https://zenodo.org/record/1240603",
					"latest": "https://zenodo.org/api/records/1240603",
					"latest_html": "https://zenodo.org/record/1240603",
					"self": "https://zenodo.org/api/records/1240603"
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
							"affiliation": "Tel Aviv University, Tel Aviv, Israel",
							"name": "Renan, Ittai"
						},
						{
							"affiliation": "Leuphana University Lüneburg, Lüneburg, Germany",
							"name": "Assmann, Thorsten"
						},
						{
							"affiliation": "Tel Aviv University, Tel Aviv, Israel",
							"name": "Freidberg, Amnon"
						}
					],
					"description": "<p>The south-west Palaearctic Graphipterus serrator group is revised. The systematic concept of the G. serrator group has undergone many changes during the last two centuries, and several different classifications have been published in recent decades. Here, the numerical taxonomy approach is used with the morphological characterization similarity level of the sympatric taxa in order to delimit allopatrically occurring taxa at the species and subspecies level. A key to the species and distribution maps are provided along with analyses of the conservation status and habitat preferences of the taxa. The Graphipterus serrator group currently comprises 16 taxa. Five new species are described: Graphipterus magnus Renan &amp; Assmann, sp. n., Graphipterus mauretensis Renan &amp; Assmann, sp. n., Graphipterus piniamitaii Renan &amp; Freidberg, sp. n., Graphipterus sharonae Renan &amp; Assmann, sp. n., and Graphipterus stagonopsis Renan &amp; Assmann, sp. n. In addition, five taxa are revalidated to full species status: Graphipterus heydeni Kraatz, 1890, stat. rest. (lectotype designated), Graphipterus multiguttatus (Olivier, 1790), stat. rest. (lectotype designated), Graphipterus peletieri Laporte de Castelnau, 1840, stat. rest. (the frequently used name lepeletieri is an error), Graphipterus rotundatus Klug, 1832, stat. rest. (lectotype designated), and Graphipterus valdanii Guérin-Méneville, 1859 stat. rest., and a full species status is proposed for Graphipterus reymondi Antoine, 1953, stat. n. One new synonymy is proposed: Graphipterus kindermanni Chaudoir, 1871, syn. n. of Carabus multiguttatus Olivier, 1790. Lectotype designations were made for Graphipterus heydeni, Graphipterus minutus Dejean, 1822, Graphipterus multiguttatus, and Graphipterus rotundatus. Neotype designations were made for Graphipterus reichei Guérin-Méneville, 1859, Graphipterus intermedius Guérin-Méneville, 1859, and Graphipterus valdanii Guérin-Méneville, 1859.</p>",
					"doi": "10.3897/zookeys.753.22366",
					"imprint": {
						"publisher": "Pensoft Publishers"
					},
					"journal": {
						"issue": "",
						"pages": "23-82",
						"title": "ZooKeys",
						"volume": "753"
					},
					"keywords": [
						"Animalia",
						"Arthropoda",
						"Insecta",
						"Coleoptera",
						"Caraboidea",
						"Carabidae",
						"Graphipterus",
						"Graphipterus serrator",
						"Allopatry",
						"conservation status",
						"ground beetles",
						"Harpalinae",
						"Lebiini",
						"species delimitation",
						"sand dunes",
						"sympatry"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2018-04-26",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "1240603"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "1240602"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Taxonomic revision of the Graphipterus serrator (Forskål) group (Coleoptera, Carabidae): an increase from five to 15 valid species"
				},
				"owners": [
					1161
				],
				"revision": 5,
				"stats": {
					"downloads": 21,
					"unique_downloads": 21,
					"unique_views": 8,
					"version_downloads": 21,
					"version_unique_downloads": 21,
					"version_unique_views": 8,
					"version_views": 8,
					"version_volume": 530114529,
					"views": 8,
					"volume": 530114529
				},
				"updated": "2020-01-20T15:17:18.360761+00:00"
			},
			{
				"conceptrecid": "782136",
				"created": "2017-05-12T14:43:44.328755+00:00",
				"doi": "10.3897/zookeys.100.1524",
				"files": [
					{
						"bucket": "64ec63e7-af98-418f-a26d-5e1bac434a2d",
						"checksum": "md5:efb961c9fce545ca955315f65355ec76",
						"key": "ZK_article_2417.pdf",
						"links": {
							"self": "https://zenodo.org/api/files/64ec63e7-af98-418f-a26d-5e1bac434a2d/ZK_article_2417.pdf"
						},
						"size": 965439,
						"type": "pdf"
					},
					{
						"bucket": "64ec63e7-af98-418f-a26d-5e1bac434a2d",
						"checksum": "md5:466c9ca9669f85ade8ad03c6734ae3bc",
						"key": "ZK_article_2417.xml",
						"links": {
							"self": "https://zenodo.org/api/files/64ec63e7-af98-418f-a26d-5e1bac434a2d/ZK_article_2417.xml"
						},
						"size": 402493,
						"type": "xml"
					}
				],
				"id": 576875,
				"links": {
					"badge": "https://zenodo.org/badge/doi/10.3897/zookeys.100.1524.svg",
					"bucket": "https://zenodo.org/api/files/64ec63e7-af98-418f-a26d-5e1bac434a2d",
					"doi": "https://doi.org/10.3897/zookeys.100.1524",
					"html": "https://zenodo.org/record/576875",
					"latest": "https://zenodo.org/api/records/576875",
					"latest_html": "https://zenodo.org/record/576875",
					"self": "https://zenodo.org/api/records/576875"
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
							"affiliation": ", ,",
							"name": "Zinovyev, Evgeniy"
						}
					],
					"description": "The distribution of beetles at the end of the Middle Pleninglacial (=terminal Quaternary) was examined based on sub-fossil material from the Ural Mountains and Western Siberia, Russia. All relevant localities of fossil insects have similar radiocarbon dates, ranging between 33,000 and 22,000 C14 years ago. Being situated across the vast territory from the southern Ural Mountains in the South to the middle Yamal Peninsula in the North, they allow latitudinal changes in beetle assemblages of that time to be traced. These beetles lived simultaneously with mammals of the so-called \"mammoth fauna\" with mammoth, bison, and wooly rhinoceros, the often co-occurring mega-mammalian bones at some of the sites being evidence of this. The beetle assemblages found between 59° and 57°N appear to be the most interesting. Their bulk is referred to as a \"mixed\" type, one which includes a characteristic combination of arcto-boreal, boreal, steppe and polyzonal species showing no analogues among recent insect complexes. These peculiar faunas seem to have represented a particular zonal type, which disappeared since the end of the Last Glaciation to arrive here with the extinction of the mammoth biota. In contrast, on the sites lying north of 60°N, the beetle communities were similar to modern sub-arctic and arctic faunas, yet with the participation of some sub-boreal steppe components, such as Poecilus ravus Lutshnik and Carabus sibiricus Fischer-Waldheim. This information, when compared with our knowledge of synchronous insect faunas from other regions of northern Eurasia, suggests that the former distribution of beetles in this region could be accounted for both by palaeo-environmental conditions and the impact of grazing by large ruminant mammals across the so-called \"mammoth savannas\".",
					"doi": "10.3897/zookeys.100.1524",
					"journal": {
						"issue": "",
						"pages": "149-169",
						"title": "ZooKeys",
						"volume": "100"
					},
					"keywords": [
						"Carabidae",
						"Coleoptera",
						"sub-fossil beetles",
						"fauna change",
						"insect assemblages"
					],
					"license": {
						"id": "CC-BY-4.0"
					},
					"publication_date": "2011-05-20",
					"relations": {
						"version": [
							{
								"count": 1,
								"index": 0,
								"is_last": true,
								"last_child": {
									"pid_type": "recid",
									"pid_value": "576875"
								},
								"parent": {
									"pid_type": "recid",
									"pid_value": "782136"
								}
							}
						]
					},
					"resource_type": {
						"subtype": "article",
						"title": "Journal article",
						"type": "publication"
					},
					"title": "Sub-fossil beetle assemblages associated with the \"mammoth fauna\" in the Late Pleistocene localities of the Ural Mountains and West Siberia"
				},
				"owners": [
					1161
				],
				"revision": 8,
				"stats": {
					"downloads": 23,
					"unique_downloads": 22,
					"unique_views": 12,
					"version_downloads": 23,
					"version_unique_downloads": 22,
					"version_unique_views": 12,
					"version_views": 12,
					"version_volume": 22205097,
					"views": 12,
					"volume": 22205097
				},
				"updated": "2020-01-20T17:17:27.451289+00:00"
			}
		],
		"from": 1,
		"to": 30,
		"prevpage": 0,
		"nextpage": 2
	},
	"cached": null,
	"report": {
		"error": {
			"data": null,
			"isBoom": true,
			"isServer": true,
			"output": {
				"statusCode": 500,
				"payload": {
					"statusCode": 500,
					"error": "Internal Server Error",
					"message": "An internal server error occurred"
				},
				"headers": {
				}
			}
		},
		"msec": 0.12305259704589844
	}
}
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
