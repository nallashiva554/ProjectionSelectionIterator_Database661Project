Iterators are used by the clients or other high-level programs to instream tuples/ data from the page. It reads the tuples of the relation located on the storage in the background and returns the tuples one by one to the page thus hiding the database low-level page handling.

Base Iterator is the basic iterator that reads the storage of the relation and iterates through the tuples, returning all the available tuples one-by-one until the end of the page allocated to the relation is reached. When there are multiple pages, the iterator uses the header information to fetch the nextPage information and positions the pointer to the start of the next page.

Projection-Selection Iterator uses the Base Iterator and returns the tuples that meet the selection criteria as specified in the XML file of the expression tree for the corresponding relation. Each tuple returned will contain only the attributes specified for projection in the XML file of the Expression tree.

Instructions:
--------------
CompileJava_2_Deep.bat support jdk1.7.0_75 Version of Java. If you have to use it, install this version on your machine at C:\Program Files\Java\ Path
OR
change you version instead of jdk1.7.0_75 to your machine support version.