# Finding-all-documents-which-contains-one-or-two-search-keywords

Credits to idea: Youtube [video](https://youtu.be/VjgLdhcmB7I?t=6517)

The text files in *docs* are taken from [Wikipedia](https://www.wikipedia.org/). 

**Problem Statement:** Given one or two search keywords, we have to return the list of documents that contain those keywords. If the search query contains two keywords, then we return those documents where keywords are present in the document side-by-side.
**Example:** Suppose document1 contains “Excitement replaced fear **until the** final moment.” and document2 contains “**until** can be used in **the** following ways.” as text. Now if the search query is “**until the**”, then only doument1 is returned as result.
**Procedure:** Ten Wikipedia documents are stored in a text format in the docs folder. In the first step, namely preprocessing, a dictionary is build with word and two side-by-side words in a document as a key and a document name as a value. The value in the dictionary is converted to a set to remove duplicates. The dictionary is stored in a pickle format.
In the next step, when the user queries using search keyword(s), a list of documents containing search keyword(s) are displayed. If the query keyword(s) are not present then a message saying query keyword(s) not present is displayed.
The motivation to use a dictionary is because the average case time complexity for search in the dictionary is O(1) [source](https://wiki.python.org/moin/TimeComplexity).
Linkedin post can be found [here](https://www.linkedin.com/posts/activity-6766261745024667648-vZJw).
Demo video on vimeo can be found [here](https://vimeo.com/511881280).
