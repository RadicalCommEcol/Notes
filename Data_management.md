# Recommendations for a good data management:

1.	Plan ahead: Ensuring [FAIR](https://www.go-fair.org/fair-principles/) data is easier if you have a plan, and you build your datasets right from the beginning. [Best practices](https://old.dataone.org/best-practices) include always preserving the raw data, scripting all data processing steps so the cleaning process is reproducible (or using manual alternatives such as [Open Refine](https://openrefine.org/), and using [tidy data](http://vita.had.co.nz/papers/tidy-data.pdf) formats.  

2.	Use version control and backup protocols: Your data and code evolve with the project. Using version control tools (e.g. [git](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F)) helps trace all the steps done, and when synced online serves as a backup in case of data loss. The use of [github](https://github.com/) simplifies and automates the process (tutorial at [happygitwithr](https://happygitwithr.com/)), but at a minimum all major steps should be versioned (e.g. data_v0.1, data_v1.0) and backed up in independent data servers.   

3.	Think on (automated) unit testing: Errors happen, even in simple tasks like data entry. Follow [best practices](https://doi.org/10.1080/00031305.2017.1375989) on data organization. Design spreadsheets with real-time data validation to minimise errors when typing the data. And perform post data-entry quality control too: testing for impossible or unlikely data points before using and releasing a dataset is crucial. You can do that manually but it is better when done automatically, for which there are several [dedicated packages in R](https://cran.r-project.org/web/packages/validate/vignettes/JSS_3483.pdf). For complex datasets, automatic integration tools are available (e.g. [github actions](https://lab.github.com/githubtraining/github-actions:-continuous-integration))  

4.	Use non-proprietary formats to release your data: Accessible means you can open and read the data without proprietary software. Plain text files such as .csv are also more lightweight (data storage size is directly linked to energy consumption and environmental problems), durable, and hard to corrupt.  

5.	Use metadata standards: No data should be released without proper metadata. Ideally, this metadata has a human-readable summary but is composed of machine-readable code. There are generic metadata options such as [dataspice package](https://github.com/ropenscilabs/dataspice), or the more complete [EML](https://eml.ecoinformatics.org/) standard for ecology. Only that way data will be discoverable and interoperable in the near future.  

6.	Release data with a DOI and a license: Data is being lost at incredible rates. Local hard drives, dedicated webpages, and servers (e.g. a github repository) are not forever and can be modified. A Digital Object Identifier ([DOI](https://www.doi.org/)) associated with a standard repository ensures the availability in the future of the original files. Along with the release, adding a license is basic to ensure users know what can they do with the data (e.g. [Open data licenses](https://opendatacommons.org/licenses/)).   

7.	Use the most appropriate repository for your data: There is a growing number of permanent data repositories. [Zenodo](https://zenodo.org/), [Figshare](https://figshare.com/) or [Dryad](https://datadryad.org/) provide DOI and are generic repositories that can accommodate different types of data, but thematic repositories exist such as [Gbif](https://www.gbif.org/) for occurrence data, or [Genbank](https://www.ncbi.nlm.nih.gov/genbank/) for genetic data. Using those will increase the re-use of your data.   