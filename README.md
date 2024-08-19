# Journal Citation Lengths

Supplementary data for the paper Citation Distance Matters: Towards a New Metric for Evaluating Journal Impact - Barnes et al. (2024)

## How to cite

## Source

Data for the journal citation network was collected via a full data dump from [OpenAlex](https://openalex.org/) in October 2023. 

The validation data sets were collected from the [Norwegian Journal Rank](https://kanalregister.hkdir.no/publiseringskanaler/Forside.action?request_locale=en), [Finnish Journal Ranks](https://julkaisufoorumi.fi/en/publication-forum), [SCImago Journal Rank](https://www.scimagojr.com/journalrank.php), [JCR Suppressed Journals](https://jcr.help.clarivate.com/Content/title-suppressions.htm) and [CIDRE Anomalous Journals](https://www.nature.com/articles/s41598-021-93572-3).

Open access to all data sets in the [data](./data) folder.

## Summary of data

The journal citation network was built from meta data for 32,217,303 papers: 

| Feature | Type | Description |
|----------------------|-------------------------------|--------------------------------------------------------|
| article id | int | unique article identifier |
| publication year | int | year published |
| reference list | list of ints | article ids referenced |
| publishing journal id | int | unique journal identifier |

In total, the journal citation network contained 21,366 with the following metadata:

| Feature | Type | Description |
|----------------------|-------------------------------|--------------------------------------------------------|
| journal id | int | unique journal identifier |
| ISSN | int | online and print ISSN numbers |
| title | string | journal title |
| discipline | list | discipline name and proportion of journal articles in discipline |
| # 2020 | int | number of articles published in 2020 |
| # 2021 | int | number of articles published in 2021 |

## Code files

Python code files with exploratory analysis of the data sets, engineering of five unique metrics, and results visualization [code](./code) folder.

## Supplementary figures

Please see [code](./code) files for our five metrics proposed in the paper for all data distributions.
