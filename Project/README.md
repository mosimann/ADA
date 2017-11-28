# Do Markets Follow Patents?

# Abstract

Protecting intellectual property through patents is a cornerstone of Western innovation. Yet, there is no global consensus on whether patents promote or stall innovation, and whether that innovation is in turn rewarded by markets. In this project, we propose to observe how companies applying for and being granted patents relates to their market capitalization and earnings. We build a graph database by combining a patent citations dataset and associated metadata. We then explore the resulting dataset to extract insight into companies' valuations in relation to their patent portfolio. Finally, we dig deeper into select companies to correlate patent activity with earnings and financial indicators such as stock prices.

# Research questions
* What are the major patent holders? Are these highly valued companies?
* Is there a relation between companies' valuation and number of patents in their portfolios?
* Are there key patents (i.e. influential patents) which significantly impacted market capitalization?
* Can patent-related events (e.g., the granting of a patent) influence earnings and share prices?

# Dataset

## Datasets

The two suggested datasets:

* http://snap.stanford.edu/data/cit-Patents.html
* http://www.patentsview.org/api/doc.html

Extra datasets:

* http://www.nber.org/patents/
* http://etfdb.com/history-of-the-s-and-p-500/
* https://wrds-web.wharton.upenn.edu/wrds/
* Wikipedia (manual)

## Data Wrangling

1. Use the original datasets to create a graph of citations. Note: The patents citations dataset is in NET format, i.e. edge list, and contains only structural information.
2. Enrich the citation graph with metadata using nber.org. In particular, we expect to have company, inventors, sectors, types, and various date information. This information will be stored in a separate dataframe.
3. Build a financial (markets) dataset using etfdb.com and wrds-web.wharton.upenn.edu.

