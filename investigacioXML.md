# MP03_UF5


# Com passar de XML a JAVA


# DOM:
- Qué és?
DOM is a tree-based interface that models an XML document as a tree of nodes, upon which the application can search for nodes, read their information, and update the contents of the nodes.

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200001635-86f2316a-2341-4e27-9926-141edbd132fd.png>
</p>
     

- Com funciona?
- Classes necessàries
- Excepcions que s'han de controlar
- Codi d'exemple de lectura des de fitxer
- Codi d'exemple d'escriptura a fitxer

# SAX:

SAX is an event-driven interface. The application registers with the parser various event handlers, alias knowed as Simple API for XML
SAX (Simple API for XML) is an event-driven online algorithm for parsing XML documents, with an API developed by the XML-DEV mailing list. SAX provides a mechanism for reading data from an XML document that is an alternative to that provided by the Document Object Model (DOM).


# DIFERENCIES ENTRE DOM I SAX
SAX Parser ea lets

Itis called a Simple API for XML
Parsing

It's an event-based parser.

SAX Parser is slower than DOM
Parser.

Best for the larger sizes of files.

It is suitable for making XML files in
Java.

The internal structure can not be
created by SAX Parser.

Itis read-only.

In the SAX parser backward
navigation is not possible.

Suitable for efficient memory.

Asmall part of the XML file is only
loaded in memory.

It is called as Document Object
Model

It stays ina tree structure.



DOM Parser is faster than SAX
Parser.

Best for the smaller size of files.

Itis not good at making XML files in
low memory.

The internal structure can be
created by DOM Parser.

It can insert or delete nodes.

In DOM parser backward and
forward search is possible

Suitable for large XML document.

It loads whole XML documents in
memory.

 



# XPath:
- Què és XPath?
XPath (XML Path Language) is a language that allows you to build expressions that traverse and process an XML document. The idea is similar to regular expressions to select parts of a text without attributes (plain text). XPath allows you to search and select taking into account the hierarchical structure of XML. XPath was created for use in the XSLT standard, in which it is used to select and examine the structure of the input document of the transformation. XPath was defined by the W3C consortium.

- Què puc fer amb XPath?
XPath stands for XML Path Language. It uses a non-XML syntax to provide a flexible way of addressing (pointing to) different parts of an XML document. It can also be used to test addressed nodes within a document to determine whether they match a pattern or not.

- Posa un exemple de com consultar els CDs anteriors a 1990


# XQuery:
- Què és XQuery?
XQuery is a query language that allows querying and extracting information stored in XML format.
It could be said that XQuery is to XML the same as SQL is to relational databases

- Què puc fer amb XQuery?
XQuery was devised primarily as a query language for data stored in XML form. So its main role is to get information out of XML databases — this includes relational databases that store XML data, or that present an XML view of the data they hold.

- Posa un exemple de com consultar els CDs més barats de 10$

