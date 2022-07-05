# Apache Solr - Searching queries

The script aims to submit a set of queries to the collection indexed in Apache Solr, based on an [XML file](https://github.com/lucaslioli/solr-query-script/blob/main/queries_example.xml). The output is a ranking of the top 100 most relevant documents to each topic. Each query is searched using _proximity search_, and it is also possible to determine the usage of _description_ and _narrative_ to search.

Repostory to persist the code used in the experimetns from the paper **Evaluating and Mitigating the Impact of OCR Errors on Information Retrieval: A Case Study in the Geoscientific Domain**, submitted to **International Journal on Digital Libraries**.

Authors: Lucas Lima de Oliveira, Danny Suarez Vargas, Antônio Marcelo Azevedo Alexandre, Fábio Corrêa Cordeiro, Diogo da Silva Magalhães Gomes, Max de Castro Rodrigues, Regis Kruel Romeu, Viviane Pereira Moreira.

- REGIS collection link: https://github.com/Petroles/regis-collection
- REGIS Gold Standard link: https://github.com/lucaslioli/regis-collection-gs


## Requirements

* [Apache Solr installation](https://lucene.apache.org/solr/guide/7_7/installing-solr.html)
* Python 3.6+
* PIP Packages: untangle; xmltodict; requests.

## Execution

```
python3 execute_queries.py collectionName lang queries_example.xml title
```
