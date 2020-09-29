# Online markets for illicit drugs in Georgia

## The report
This document presents the findings of a six-month study into online markets for illicit drugs in Georgia. It examines Matanga, a cryptomarket platform that facilitates the anonymous sale of drugs in Georgia and countries of the CIS. It finds a diverse and active marketplace with 16 unique substances listed for sale in the country, generating nearly 1.6 million USD in revenue over a 194-day period. The study document consists of the following:

- [Online Markets for Illicit Drugs in Georgia](https://crrc.ge/uploads/tinymce/documents/PolicyBriefs/Online%20Markets%20for%20Illicit%20Drugs%20in%20Georgia%20-%20Report%20-%20FINAL.pdf): The main report
- [Annex 1: Methodological Annex](https://crrc.ge/uploads/tinymce/documents/PolicyBriefs/Online%20Markets%20for%20Illicit%20Drugs%20in%20Georgia%20-%20Annex%201%20-%20Methodological%20Annex.pdf): An overview of the study's methodology
- [Annex 2: Per substance summary data](https://crrc.ge/uploads/tinymce/documents/PolicyBriefs/Online%20Markets%20for%20Illicit%20Drugs%20in%20Georgia%20-%20Annex%202%20-%20Substance%20Summary%20Data.pdf): Summarizing all substances found


## Replication code and source data

This repository contains the source data and replication code for the report "Online markets for illicit drugs in Georgia". The repository consists of the following files and folders:
- [scrape.py](https://github.com/crrcgeorgia/matanga/blob/master/scrape.py): the scraper for Matanga. This ceased working and was repaired periodically throughout the study as changes to Matanga broke the script. It has not been updated since ceasing functioning in mid-August 2020 and will require further adjustment to operate.
- [clean.py](https://github.com/crrcgeorgia/matanga/blob/master/clean.py): consolidation of data and post processing
- [sales.py](https://github.com/crrcgeorgia/matanga/blob/master/sales.py): sales estimation function, called from [clean.py](https://github.com/crrcgeorgia/matanga/blob/master/clean.py)
- [utils.py](https://github.com/crrcgeorgia/matanga/blob/master/utils.py): utility functions, used to avoid cluttering [clean.py](https://github.com/crrcgeorgia/matanga/blob/master/clean.py)
- [policy_brief.py](https://github.com/crrcgeorgia/matanga/blob/master/policy_brief.py): Anaylsis of data derived from the above.

This code is presented as was at the time of study completion and comes with no guarantees. If you are interested in replicating the analysis, please contact the author at [i.goodrich@crrccenters.org](mailto:i.goodrich@crrccenters.org).

Source data for the study is also provided in the following folders:

- [SCRAPED](https://github.com/crrcgeorgia/matanga/tree/master/DATA/INPUT/SCRAPED): Source data drawn from [scrape.py](https://github.com/crrcgeorgia/matanga/blob/master/scrape.py)
- [LISTINGS](https://github.com/crrcgeorgia/matanga/tree/master/DATA/OUTPUT/LISTINGS/CSV): All listing data following consolidation and cleaning. Observed at listing per scrape.
- [SALES](https://github.com/crrcgeorgia/matanga/tree/master/DATA/OUTPUT/SALES/CSV): All sales data following sales estimation. Observed at listing per day.

## Bibtex

```
@misc{goodrich_online_2020,
	address = {Tbilisi, Georgia},
	title = {Online markets for illicit drugs in {Georgia}: replication code and source data},
	url = {https://github.com/crrcgeorgia/matanga},
	publisher = {CRRC Georgia},
	author = {Goodrich, Ian},
	month = sep,
	year = {2020}
}
```
