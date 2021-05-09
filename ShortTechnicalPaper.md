# Full Text Search
This paper talks about full text search and the *scalability/performance* issues of various software/databases dedicated to perform full-text-search
but first let's learn about what a full-text-search is in brief

Wikipedia article defines Full-Text-Search as **Techniques for searching a single stored document or a collection, in full-text-database**.
*Full-text-database* refers to a database where full-text data is stored eg:- storing all the words in a book, storing entire magzine or entire newspaper. Here the search engine has to scan through all the words in all the documents in order to match the user-specified text.
If search is done in small number of documents then search engines might directly scan through contents of document to match the text. But if the data is huge 
then full-text-search will perform two tasks **indexing** and **scaling**. In indexing stage each word of document will be indexed along with that their relative
position in the document will also be noted. Indexer have a feature of ignoring common words(a,an,the,as,is)
