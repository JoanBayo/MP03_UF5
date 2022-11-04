# MP03_UF5
# Com passar de XML a JAVA


# DOM
DOM parser is a tree-based API. A tree-based API is centered around a tree structure and therefore provides interfaces on components of a tree (which is a DOM document) such as Document interface,Node interface, NodeList interface, Element interface, Attr interface and so on.

A DOM parser creates a tree structure in memory from the input document and then waits for requests from client. A DOM parser always serves the client application with the entire document no matter how much is actually needed by the client. With DOM parser, method calls in client application have to be explicit and forms a kind of chained method calls.

 

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200001635-86f2316a-2341-4e27-9926-141edbd132fd.png>
</p>
     
In below example code, I am assuming that user is already aware of the structure of employees.xml file (it’s nodes and attributes); So example directly start fetching information and start printing it in console. In real life application, we will use this information for some real purpose rather than printing it on console and leave.

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200003679-4edc8594-ba4a-41c9-9c5b-fec7ef97d012.png>
</p>

Program Output:
     
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200003808-e599ce9d-29e2-4661-aec5-8354d17b2a4c.png>
</p>




# SAX:

SAX parser is a event-based API. Usually an event-based API provides interfaces on handlers. There are four handler interfaces, ContentHandler interface, DTDHandler interface, EntityResolver interface and ErrorHandler interface.

SAX parser does not create any internal structure. Instead, it takes the occurrences of components of a input document as events, and tells the client what it reads as it reads through the input document. SAX parser serves the client application always only with pieces of the document at any given time. With SAX parser, some custom methods are called [ “callback” methods ] when some certain events occur during parsing on xml document. These methods do not have to be called explicitly by the client, though we could call them explicitly.

Now in the below example code, let us write some code to test whether our handler is actually working.

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200005982-f6867a0a-cff6-4eeb-a6d0-98cb584f22d2.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200006674-cbd421f6-4493-4c28-9ad5-e41ae81d4127.png>
</p>



# DIFERENCE BETWEEN DOM AND SAX

Let’s list down an easy to remember short list of differences.

DOM 

- Parses entire document
- Represents result as a tree
- Lets you search tree
- Lets you modify tree
- Good for reading data/configuration files


SAX

- Parses until you tell it to stop
- Fires event handlers for each:
- Start tag
- Tag body
- End tag
- Low level APIs
- Good for very large documents, especially if you only care about very small portions of the document.


# HOW TO CHOOSE BETWEEN DOM AND SAX?

Ideally a good parser should be fast ,space efficient, rich in functionality and easy to use . For example, a DOM Parser is rich in functionality , but it is space inefficient when the document is huge, and it takes a little bit long to learn how to work with it.

What’s more, it runs faster and is easier to learn than DOM Parser because its API is really simple. But from the functionality point of view, it provides less functions which mean that the users themselves have to take care of more, such as creating their own data structures.

I think the answer really depends on the characteristics of your application and your current requirements.



# XPath:
- Què és XPath?
XPath (XML Path Language) is a language that allows you to build expressions that traverse and process an XML document. The idea is similar to regular expressions to select parts of a text without attributes (plain text). XPath allows you to search and select taking into account the hierarchical structure of XML. XPath was created for use in the XSLT standard, in which it is used to select and examine the structure of the input document of the transformation. XPath was defined by the W3C consortium.



- Què puc fer amb XPath?
XPath stands for XML Path Language. It uses a non-XML syntax to provide a flexible way of addressing (pointing to) different parts of an XML document. It can also be used to test addressed nodes within a document to determine whether they match a pattern or not.


- Posa un exemple de com consultar els CDs anteriors a 1990


# XQuery:
- Què és XQuery?
XQuery is a query language that allows querying and extracting information stored in XML format. It could be said that XQuery is to XML the same as SQL is to relational databases

- Què puc fer amb XQuery?
XQuery was devised primarily as a query language for data stored in XML form. So its main role is to get information out of XML databases — this includes relational databases that store XML data, or that present an XML view of the data they hold.

- Posa un exemple de com consultar els CDs més barats de 10$




# REFERENCES:
https://howtodoinjava.com/java/xml/read-xml-dom-parser-example/
https://howtodoinjava.com/java/xml/sax-parser-read-xml-example/

