# Do Markets Follow Patents?

# Abstract

By using datasets containing patents content and citations, this project aims to observe how these patents can predict innovation trends, product launches and popularity of an area. The idea is to see if patents say more than the declaration and appropriation of a new concept, and if patent dynamics can be linked to firm dynamics. If such a hypothesis would be confirmed, it would mean that this analysis strategy could be used nowadays to help investors in stock market, or describe and predict market states.

# Research questions
* 
* What are the major innovation trends?
* Does patent activity in a particular area correlate with product launches? How long after patenting do products come out? Does the patent application type influence the release of products?
* Do fewer granted patents in a given area indicate economic slowdown?
* Are patent processing times indicative of popularity of the area? Do they vary across various domains?

# Dataset
## Datasets
The two suggested datasets:

* http://snap.stanford.edu/data/cit-Patents.html
* http://www.patentsview.org/api/doc.html

Extra datasets of possible interest:

* http://www.nber.org/patents/
* https://sites.google.com/site/patentdataproject/Home/downloads

Datasets for enrichment:

* Wikidata
* Freebase/Knowledge Graph

## Data Wrangling
1. Use the original datasets to create a graph of citations. Note: The patents citations dataset is in NET format, i.e. edge list, and contains only structural information.
2. Enrich the citation graph with metadata using patentsview.org and/or nber.org. In particular, we expect to have company, inventors, sectors, types, and various date information. This information will be attached to the nodes. A possible challenge might be to keep the total data size under control.  
3. 

# A list of internal milestones up until project milestone 2
1. Due to 7.11: Understand the dataset and identify useful information 
2. Due to 14.11: Create categories and sort patents according to them. This will allow us to identify the patent activity in particular areas. 
3. Due to 21.11: Collect data on product launches and economy of enterprise
4. Due to 28.11: Link the patent dataset with the information about companies

# Questions for TAs
Add here some questions you have for us, in general or project-specific.
