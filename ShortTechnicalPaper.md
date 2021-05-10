# Full Text Search
This paper talks about full text search and the *scalability/performance* issues of various software/databases dedicated to perform full-text-search
but first let's learn about what a full-text-search is in brief.

Wikipedia article defines Full-Text-Search as **Techniques for searching a single stored document or a collection, in full-text-database**.
*Full-text-database* refers to a database where full-text data is stored eg:- storing all the words in a book, storing entire magzine or entire newspaper. Here the search engine has to scan through all the words in all the documents in order to match the user-specified text.
If search is done in small number of documents then search engines might directly scan through contents of document to match the text. But if the data is huge 
then full-text-search will perform two tasks **indexing** and **scaling**. In indexing stage each word of document will be indexed along with that their relative
position in the document will also be noted. Indexer have a feature of ignoring **stop words**(a,an,the,as,is,to,for .etc) along with that indexer might **stem** 
words which represent same thing for different instance, words like 'take','took','taken' will be index into single word concept 'take'.

We will now discuss performance and scalibilty issues of some search engines performing full text search.

## Elastic Search 
Elastic Search has some following primary features.

### Open Source
Anybody can download it use it without paying any fee or having any license.

### Scalable
As the name itself suggest 'Elastic' means that this engine was mainly designed to be scalable(increase like elastic) across multiple nodes. if more nodes are
added with time then this search engine is designed to handle such scalability.

### Performance
It's comparatively more fast than other full-text-search engines.

### Document Oriented
It stores data in document and doesn't use any schema or table. Data is presented in JSON format.

### Schema Less
As the data stored is in form of documents it doesn't have tables or schema hence it's schema less.

### Autocompletion
It supports autocompletion and also instant search. So when you type query it will automatically suggest queries to auto-type.

### MultiLingual
It's available in various other langauges to be used by diverse users.

#### Some advantages of using Elasticsearch are as follows:
* It's easy to scale up in Elasticsearch as it's distributed and document oriented.
* Multi-tenancy; where multiple nodes/users can access same software instance, is easily handled in elastic search.
* It's 'real time'; means the document as soon as it's added becomes searchable.
* It's build on java so it's compatible to run anywhere.
* It supports all document type except those that do not support text rendering.
* It's documentation is available in many languages for people of different regions to use it.

#### Some disdvantages of Elasticsearch:
* It's not a good data store like hadoop or MongoDB. it works well for small use but when data is in TB's per day it loses data.
* It's not simple and very difficult to learn as query syntax is not human language friendly, also documentation is very poor.
* Problem of **split-brain** might occur due to which data might get split and get corrupted.

### Conclusion on Elasticsearch
It's very fast, scalable, handle multi-tenancy easily but it's not a good data store(when data is very very large in TB's per day) also there is no support for
transaction or processing on data manipulation along with that it's not very simple to learn like 'out of box'. So if user's major requirement is Scalability
and fast search, user must definately choose Elasticsearch.

## Lucene
Lucene is another full text search engine and has following features.

### Open Source
It's open source, no need of paying fee or having license to access search engine.

### Speed
It's faster than any other full text search engines as it's incremnetal indexing is faster than batch indexing.

### Fuzzy Search
It will try to locate to exact document even when the user specified string doesn't match the output result(this search technique is called fuzzy search).

### Recommendation Systems
It can been used to implement recommendation systems to recommend similar documents similar to user specified document.

### Accurate Search
It supports power queries including proximity queries, phrase queries and range queries to make accurate searching.

**Let's talk about some advantages of using Lucene**.
* It has large and active development community with large number of developers.
* It's fast as it's development language is java.
* It's search algorithm provides most accurate search results.
* It's offers better memory optimization.
* available for different programming languages

**Some disadvantages of lucene**:
* It's real time search is slow, there is a time delay between indexing to searchable.
* Other search engines have better scalability scheme.
* 


