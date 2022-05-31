# Apache Solr - Searching queries

The script aims to submit a set of queries to the collection indexed in Apache Solr, based on an [XML file](https://github.com/lucaslioli/regis-collection-gs/blob/main/queries_example.xml). The output is a ranking of the top 100 most relevant documents to each topic. Each query is searched using _proximity search_, and it is also possible to determine the usage of _description_ and _narrative_ to search.

Repostory to persist the code used in the experimetns from the paper **Evaluating the Impact of OCR Quality on Information Retrieval: A Case Study in the Geoscientific Domain**.

Lucas Lima de Oliveira, Danny Suarez Vargas, Viviane Pereira Moreira, Antônio Marcelo Azevedo Alexandre, Fábio Corrêa Cordeiro, Diogo da Silva Magalhães Gomes, Max de Castro Rodrigues. "Evaluating the Impact of OCR Quality on Information Retrieval: A Case Study in the Geoscientific Domain".

- REGIS collection link: https://github.com/Petroles/regis-collection
- REGIS Gold Standerd link: https://github.com/lucaslioli/regis-collection-gs


## Requirements

* [Apache Solr installation](https://lucene.apache.org/solr/guide/7_7/installing-solr.html)
* Python 3.6+
* PIP Packages: untangle; xmltodict; requests.

## Execution

```
python3 execute_queries.py collectionName lang queries_example.xml title
```