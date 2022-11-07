# MP03_UF5 Com passar de XML a JAVA


# DOM
DOM parser is a tree-based API. A tree-based API is centered around a tree structure and therefore provides interfaces on components of a tree (which is a DOM document) such as Document interface,Node interface, NodeList interface, Element interface, Attr interface and so on.

A DOM parser creates a tree structure in memory from the input document and then waits for requests from client. A DOM parser always serves the client application with the entire document no matter how much is actually needed by the client. With DOM parser, method calls in client application have to be explicit and forms a kind of chained method calls.

 

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200001635-86f2316a-2341-4e27-9926-141edbd132fd.png>
</p>
     
In the next exemple I try to read the XML

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190345-70425e83-d489-4946-bf06-a0c6baebaad7.png>
</p>

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190335-eb6a28ac-e0bd-487c-93e4-e4491fc18dbb.png>
</p>

Program Output:
     
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190326-0453c9cc-0d37-49f3-80cf-7f616ae71f79.png>
</p>

In the next exemple I try to write the XML
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190316-9b95226d-69b5-417b-a807-5eb279389d54.png>
</p>
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190309-980aa4bc-ad72-4233-8174-dc91369f6a2c.png>
</p>
Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200190294-87192d4a-9c55-4b86-9c3e-ed0db2b1b706.png>
</p>

# SAX:

SAX parser is a event-based API. Usually an event-based API provides interfaces on handlers. There are four handler interfaces, ContentHandler interface, DTDHandler interface, EntityResolver interface and ErrorHandler interface.

SAX parser does not create any internal structure. Instead, it takes the occurrences of components of a input document as events, and tells the client what it reads as it reads through the input document. SAX parser serves the client application always only with pieces of the document at any given time. With SAX parser, some custom methods are called [ “callback” methods ] when some certain events occur during parsing on xml document. These methods do not have to be called explicitly by the client, though we could call them explicitly.

Now in the below example code, let us write some code to test whether our handler is actually working.

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352473-d055959c-94fc-460f-9832-553f7bc6884d.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352523-829eff52-4664-45e1-a495-37d13ba083d8.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352554-4ca7ac1a-59c6-4d66-9509-5591c853f7c0.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352630-84169c2e-d628-4e10-9ee2-a0e82af170ef.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352669-f37c7478-5d4e-4716-95fd-15a6db4037ae.png>
</p>

Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352695-5daa572c-84ef-4dff-8520-6dd5e95ec0fa.png>
</p>
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200352777-224ba37d-7ca7-4118-903a-145024f86020.png>
</p>
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200338571-5d47f32c-a2ef-4026-a11f-134e4c3cdaf4.png>
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

#
#

# XPath:
- Què és XPath?
XPath (XML Path Language) is a language that allows you to build expressions that traverse and process an XML document. The idea is similar to regular expressions to select parts of a text without attributes (plain text). XPath allows you to search and select taking into account the hierarchical structure of XML. XPath was created for use in the XSLT standard, in which it is used to select and examine the structure of the input document of the transformation. XPath was defined by the W3C consortium.



- Què puc fer amb XPath?
XPath stands for XML Path Language. It uses a non-XML syntax to provide a flexible way of addressing (pointing to) different parts of an XML document. It can also be used to test addressed nodes within a document to determine whether they match a pattern or not.


- Posa un exemple de com consultar els CDs anteriors a 1990

<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200331995-4b88efa4-30de-4f61-bcfe-00838928ab9e.png>
</p>


Program Output:
<p align=center>
<img src=https://user-images.githubusercontent.com/91154202/200332135-38ddcdaa-cbb1-447f-8d02-3a791df52daf.png>
</p>


# XQuery:
- Què és XQuery?
XQuery is a query language that allows querying and extracting information stored in XML format. It could be said that XQuery is to XML the same as SQL is to relational databases

- Què puc fer amb XQuery?
XQuery was devised primarily as a query language for data stored in XML form. So its main role is to get information out of XML databases — this includes relational databases that store XML data, or that present an XML view of the data they hold.

- Posa un exemple de com consultar els CDs més barats de 10$


