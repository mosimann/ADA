# Do Markets Follow Patents?

# Abstract

Protecting intellectual property through patents is a cornerstone of Western innovation. Yet, there is no global consensus on whether patents promote or stall innovation. In particular, does innovation lead to patents or do patents lead to innovation? In this project, we propose to observe how patents applications predict technological trends, new markets, and innovation products. We build a graph data by combining a patent citations dataset [1] and associated metadata [2]. We explore the resulting graph to extract key insight into major innovation trends. We then dig deeper into select markets and companies to correlate patent activity with events such as product launches or company creation as well as financial indicators such as historical stock prices and total market value.

# Research questions
* What are the major innovation trends?
* Does patent activity in a particular area correlate with product launches? How long after patenting do products (if any) come out? Does patent application type influence the release of products?
* Do patents affect the market capitalization of companies?
* Is patent activity in a particular sector a good indicator of its total market value? Do fewer granted patents in a given area indicate economic slowdown?
* Are patent processing times indicative of popularity of the area? Do they vary across various domains?
* Is there a relationship between academic research and patent applications? In particular, are there common innovation trends or historical patterns?

# Dataset

## Datasets

The two suggested datasets:

* http://snap.stanford.edu/data/cit-Patents.html
* http://www.patentsview.org/api/doc.html

Extra datasets of possible interest:

* http://www.nber.org/patents/
* https://sites.google.com/site/patentdataproject/Home/downloads
* https://patents.google.com/
* https://scholar.google.com (Google Scholar)
* https://aminer.org/data (academic papers citations graph)

Financial information:

* https://finance.yahoo.com (Yahoo Finance)

Datasets for enrichment:

* Wikidata
* Freebase/Knowledge Graph

## Data Wrangling

1. Use the original datasets to create a graph of citations. Note: The patents citations dataset is in NET format, i.e. edge list, and contains only structural information.
2. Enrich the citation graph with metadata using patentsview.org and/or nber.org. In particular, we expect to have company, inventors, sectors, types, and various date information. This information will be attached to the nodes. We will need to use PatentsView's API to that end. A possible challenge might be to keep the total data size under control.
3. (optional -- depending on time) Derive other representations of the data. For instance, compute the connected components graph, link patents based on content (abstract), compute a bipartite graph with academic papers, create a temporal graph for patents.

# A list of internal milestones up until project milestone 2

## Week 1 (7 Nov)

* Get familiar with datasets and identify useful information.
* Begin import and enrichment process.

## Week 2 (14 Nov)

* Complete enrichment process.
* Run graph analysis algorithms on patents graph (e.g., connected components, triangles, neighborhood function).
* Explore various aggregations and trends in the data.

## Week 3 (21 Nov)

* Identify some areas, companies, topics of interest.
* Collect additional data to use for analysis and correlation, e.g., product launches, historical stock prices of companies of interest, total market values of identified areas.

## Week 4 (28 Nov)

* Combine datasets.
* Analyze and correlate.
* Determine preliminary answers to research questions.

# Questions for TAs

* Can you suggest a good dataset of product launches? We can manually gather some information (e.g., using Wikipedia), but it would help make our analysis as broad as possible to have a "pre-made" dataset.
