# Canon Shelf

In this repository, we compile literary canons and other lists of literary works in a machine-readable format. To ensure both ease of editing and human readability, we use the TSV (Tab-Separated Values) format. For other use cases, the lists can be readily converted to JSON or a range of other formats.

# Overview

- 2006-2018-1001-books
- 2024-spiegel-canon
- 2024-nzz-canon
- 2025-spiegel-canon-international

# Co-authorship, series titles, time format

Co-authorships and book series cannot be rendered adequately in a table. We modeled them as follows to make it easy to be transformed into JSON:

## Co-authorship

| List Number | Series Number | Author             | Author_Wikidata_ID | Author_GND_ID | Title         | Publication_City | Publisher     | Publisher_Wikidata_ID | Work_Goodreads_ID | Work_GND_ID  | Publication_Date |
|-------------|---------------|--------------------|--------------------|---------------|---------------|------------------|---------------|-----------------------|-------------------|--------------|------------------|
| 29          |               | Merz, Carl         | Q43866             | 115661018     | Der Herr Karl | München          | Langen Müller | Q1194235              | 4290497           | 4583169-5    | 1961             |
| 29          |               | Qualtinger, Helmut | Q45233             | 118828983     | Der Herr Karl | München          | Langen Müller | Q1194235              | 4290497           | 4583169-5    | 1961             |

## Series titles

| List Number | Series Number | Author             | Author_Wikidata_ID | Author_GND_ID | Title                      | Work_Wikidata_ID | Work_Goodreads_ID | Work_GND_ID | Publication_Date | Publication_Country |
|-------------|---------------|--------------------|--------------------|---------------|----------------------------|------------------|-------------------|-------------|------------------|---------------------|
| 25          |               | Simone de Beauvoir | Q7197              | 118507877     | Die Mandarins von Paris    | Q1214721         | 20761             |             | 1954             | Frankreich          |
| 26          | 0             | J. R. R. Tolkien   | Q892               | 118623222     | Der Herr der Ringe         | Q15228           | 3462456           | 4124318-3   | {1954;1955}      | Großbritannien      |
| 26          | 1             | J. R. R. Tolkien   | Q892               | 118623222     | Die Gefährten              | Q208002          | 3204327           | 4675755-7   | 1954             | Großbritannien      |
| 26          | 2             | J. R. R. Tolkien   | Q892               | 118623222     | Die zwei Türme             | Q332388          | 2963845           | 4675756-9   | 1954             | Großbritannien      |
| 26          | 3             | J. R. R. Tolkien   | Q892               | 118623222     | Die Rückkehr des Königs    | Q332581          | 2964424           | 4675758-2   | 1955             | Großbritannien      |
| 27          |               | Patricia Highsmith | Q270635            | 11855087X     | Der talentierte Mr. Ripley | Q472026          | 1817520           |             | 1955             | USA                 |

If multiple entries share the same list number and include series numbers, they represent parts of a series. In such cases, the entry with series number 0 is the series title. If there are no series numbers, identical list numbers indicate co-authorship of a single work.

## Time format

Publication years follow the [EDTF](https://www.loc.gov/standards/datetime/) (Extended Date/Time Format) standard. This is especially relevant for multi-volume works published over several years. In these instances, we specify the individual publication years, i.&nbsp;e. ```1970–1983``` → ```{1970,1971,1973,1983}```.

# License and Ways to Get Involved

These lists of literary works are freely available for your research and exploration under a [CC0 license](https://creativecommons.org/publicdomain/zero/1.0/). We also welcome contributions, feel free to share your own lists with us.

# Team
- Jonas Rohe ([@Fera333](https://github.com/fera333))
- Frank Fischer ([@lehkost](https://github.com/lehkost))
- Lisa Poggel ([@lipogg](https://github.com/lipogg))
- Viktor Illmer ([@v-ji](https://github.com/v-ji))
