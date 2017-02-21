Visualization Implementation 2
------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Raja Harsha Chinta

UIN: 01043488

Tool Selected for CS725-VI2: OpenRefine



Description of the tool:
----------------------------

1) OpenRefine is a standalone open source desktop application for data wrangling.

2) The program has a web user interface and starts a web server.

3) It understands data in rows-columns in one table.

4) This involves cleanup, merging duplicate data and transformation to other formats using facets.

5) All actions that were done on a dataset are stored in a project and can be replayed on another dataset.



Inconsistencies found in the data:
--------------------------------------------------------

There are numerous inconsistencies found in the dataset shared and few of them are shared below:

1) Trailing white spaces and consecutive white spaces in text columns.

2) Same String in different expressed in different notations with cases.

3) Inconsistent String representation in an abbrevated form or sometimes in full name.

4) Spelling Mistakes in Publisher Names, Jounal Titles

5) Different Publishers using same Journal title.

Steps followed to clean the data:
--------------------------------------------------------

1) Removed leading and trailing white spaces for all the columns using Common Transformation > Collapse Consecutive Whitespaces.

2) Collapsed Consecutive white spaces using Common Tranformation > Collapse Consecuting Whitespaces.

3) Applied Facet > Text Facet on Publisher and Journal Title columns to understand the counts and observe the inconsistencies.

4) Using Cluster, groups of different cell values that might be alternative representations of the same thing are identified and corrected using Merge.

5) A particular column data is verified using different varieties of clusing techniques. Few are below:
	
	key collision - fingerprint, ngram-fingerprint, metaphone3, cologne-phonetic
	nearest neighbour - levenshtein, PPM with diffent Radius and Block Chars values.

6) Some data is observed manually and corrected.

7) Same Journal Title being published by 2 Publishers is verified over internet and corrections are made.

8) Correct spellings and Notations are verified from internet wherever required.

9) More than 250 steps of transformations are applied to clean the data.


Tool used to convert the data to JSON:
--------------------------------------------------------

We have used an inbuilt tool of OpenRefine to extract the input data in a JSON file.

Export > Templting Export > Export > JSON file.

Also, an online csv to json converter is handy for this conversion. (http://www.csvjson.com/csv2json)

Benefits of OpenRefine:
--------------------------------------------------------

1) Many data wrangling tools are difficult to understand and apply user defined transformations, but OpenRefine is an easy tool to work.

2) Data remains in the user PC while using this tool, making it more reliable and secure.

3) Accepts many format of file inputs and ability to export them to many formats.

4) We can see this tool is packed with sophisticated techniques and algorithms for better accuracy and performance.

5) It is an opensource and freeware.



