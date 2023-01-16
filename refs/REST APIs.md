# REST APIs
#### status: 
#### created: 2022-07-21
---
**the representational state transaction**  paradigm its the most popular APi paradigm for the modern web apis, it expose a request-response interface . 
REST use resources . A resource is an entity that can be identified, named, addressed, or handled on the web. REST APi use those resources as data and with the help of *http* method which is use them to apply transaction to those resources 

##  Some Rules for The REST  Apis
• Resources are part of URLs, like /users.
• For each resource, two URLs are generally implemented: one
for the collection, like /users, and one for a specific element,
like /users/U123.
• Nouns are used instead of verbs for resources. For example,
instead of /getUserInfo/U123, use /users/U123.
• HTTP methods like GET, POST, UPDATE, and DELETE inform the
server about the action to be performed. Different HTTP meth‐
ods invoked on the same URL provide different functionality:

##  The Duplication effort problem

the fact that if you learn how to use an api which provided by a big company like google ,twitter won't help you to *use* the api's of other big companies . **why** , because they don't won't you to use their *competitor* api's.
the problem here is that even small and nonprofit companies follow this approach , so they create api's like no one have created, this don't help with their main goal *getting users to use their product*

>". There’s something about APIs that makes
everyone want to design their own from scratch, even when that makes no sense from
a business perspective." p 21

## Understanding Standards
the www isn't an objective thing instead it's a social construct , a set of rules that agreed upon.
this standards provide such power to increase the productivity because you just have to explain the new part of your application
we should mention that not all standards have equal force, some are well known and established and some not which are one person opinion .

### Fiat Standards
they are not really standards instead they are much more *behaviors* no one agreed to them, they *describe* how somebody thinks.
generally, the big part of the api's cake it's a fiat api, and your api under ideal circumstances will be a fiat api because your business will differ than others , But ideally a fiat standard would be just a light gloss over a number of other standards.
*we don't say your API conforms to a standard , we say it's a clone*
### Personal Standards
those are standards, a one person *opinion* , whatever, many *open standards* start of  as personal standards .
if it work for you , you can considering using it , that is someone else has done the design for you

### Corporate Standards
created by consortium and big companies to solve a problem that plug them all or just one companies trying to solve a problem for it's customers , they tend to use formal language and better defined , and they have no more force than personal standards because they just one companies or more opinion 
### Open Standards
to make an open standard it have to go through steps of processing and commenting so criticizing and suggestion for improvements , at the end the *specification* blessed by some kind of recognized standards body . this process give the standard moral force .
open standards come with *promises* and you can implement the freely 

### Requests for Comments (RFCs) and Internet Drafts
*the standards track* : the process that give as an *rfc*
an rfc start as an *internet-draft* like an experimental version you not supposed to *implement it* otherwise you have to find problems in it and give some *feedback* before 6 month . one this process is done the draft must be approved as an rfc or replaced with an updated version or the draft *expire*   
**the api's field changing rapidly and a and internet-draft better than nothing**
## Surfing The Web
### Resources and Representations
each *url* identifies a resource , when a client make a request to the url it get the *representation* underlying resource. **the client never sees a resource directly** 

### Addressability
we *expect* every site to treat every thing on it as a different resources with different urls .
the addressability principle says that every resource should have it's *own* url , if something is *important* it must have a *unique* url , and you can refer to it easily

### Short Sessions
*HTTP* sessions last for one request , the client send a req and the server send a response then it will *forget you*  as a result you could open a web page for 8 months and if you click a link , the server would respond as if you  had only waiting for a few seconds, if you don't send an HTTP request the server don't know that you *exist*
*statelessness* is mean that the server don't care about the state of the client

### Self-Descriptive Messages
When you request a web page, the HTML document you receive doesn’t just give you the immediate information you asked for. The document also helps you answer the question of what to do next.

### The Link
whenever you click a link you make a request , a GET request
the GET in the req it's an *http verb* , it's the way of a the client to tell the server **what to do to a resource** , in the case of **GET** it means "give me the representation " of this resource. in web browser GET is the *default* 

### Standardized Methods
The HTTP standard (RFC 2616) defines eight methods a client can apply to a resource , so there is a small number of standard methods
we can come up with another methods but it's a **very big deal** 
 we don't differentiate between documents by different methods instead we differentiate between them by using separate resources each one with it's own url using the defined methods 

### The Form and The Redirect
when you make a get request you have a response that your *browser* likely will *render it* , some times the browser return a **303 status code**
this tell the browser to make *another* get request to the url in the *location header* 

### Application State
when u fire up your browser u don't have any particular page loaded , this is an *empty state* , every state corresponds to a different page being open, we call this *which page you are in* **the application state**
each *transition* from one state to another corresponds to a link you decide to *follow* or a *form* you decide to *fill out*

### Resource State
it's your *adventure* from the server *perspective*
the state of the resources that is handled by the server basically we call it the resource state 
when you post a form you put the server in a new state 
the server can manipulate the application state by sending representations ("HTML Document in this case") that describe the possible state transitions .
resource state lives in the server and the client can manipulate them by sending a representation and html  form submission  *describe the desired new state* 

### Connectedness

The *Strands* of the web are the *html anchor tags and forms* each describe a get or post request ,  this is the principle of connectedness that is each web give you a way to get to the adjoining page . the web all works on *hypermedia as the engine of the application state* .
html anchor tags and form are the technique  that the server uses to explain to a  client what he can do next
*we all navigate the web by following anchor tags and filling out forms*
### The Web Is Something Special

- The web is the dominant internet application
#### the world wide web early competitors
- **The Gopher Protocol** (rfc 1436) looks like **http** without *address-ability* , then the world wide web took pity on *Gropherspace* and released the *URL* Standard(rfc 1738) which provide a gopher URL scheme "gopher://"
- **FTP** protocol for *file transfer* (rfc 959) also lake *address-ability* until rfc 1738 introduce the *ftp://* URL scheme , though, there is no machine-readable way to point to a file on an *ftp server* , ftp also have long-lived sessions , a user could login to an ftp server and tie up one of the server *TCP* connections indefinitely, in the other hand **Http** *shouldn't* tie up a TCP connection for *more than* 30 seconds

in the 1990s there is  a lot of internet protocols for searching different kinds of archives or databases, but the reality is we can do it just by sending a *GET request*  to different websites
after the web toke over there is no need to create another *application protocol* that just techies will understands, so all successful post-Web protocols do another thing the web can't do like SSH and BitTorrent,
===for most purposes, HTTP is good enough=== 

The unprecedented flexibility of the Web comes from the principles of REST

### Web APIs Lag  Behind The Web
- In *Rest* term human-readable documentation that define how to construct URLs goes against the principle of connectedness and self-descriptive messages
- it easier to find how a site work by exploring the connected self-descriptive html document than reading human readable docs , presenting the website resources in a big menu instead of an *inter-connected* web make it hard to know what one resource has to do with another
- working with new API require writing custom software , in the other hand you don't need to write a *library* to use a new website . you just use the same client you use for every other website in the world your *web-browser* 
- when APIs serve self-descriptive messages than it will become *possible* for APIs to understands each other
- When API *change* custom client of it *break* and have to be fixed but when a website change it's design , the user's grumble about the redesign then they *adapt* but their browser don't stop working
- in *REST* terms the website redesign is encapsulated in the self-descriptive html document, so a client who could understand the old design will understand the new one

### The Semantics Challenge
The Web works because human being make all the decisions about which links to follow next and which forms to fill out 
the whole point of web APIs is get things *done* without making a human sit in front of a web browser all day
a computer can *parse* HTML documtent but it can't understand it's messages
This is the biggest challenge in web API design: bridging the semantic gap between understanding a document’s structure and understanding what it means


---
### referances
- [[@richardsonRESTfulWebAPIs2013]]

## A Simple API
### HTTP GET: your safe bet
The HTTP standard says that a GET request is a request for a representation. It’s not intended to *change any resource state on the server*.
these mean that if you don't know anything about a resource just make a GET request and see it's representation because GET is a *safe method* and it will not do something disastrous , *it can change incidental things*  like incrementing a hit counter but no one make a GET to increase a counter .
at the end it all up to the designer, in old design there is no guarantee that GET is safe , they can force you to make a GET to delete some data , but this is rare in new designs . they understands that a client make a GET to see what behind the URL so they don't give it a *significant side effects* .

### How to read an HTTP Response

usually we can split the *response* to 3 entities:
- Status Code: 3 digits number which indicate how the request went 
- The Body: a Document Written in Some data Format , which the client expected to *understand* (you can think of the body as the *representation*)
- The Headers: series of key-value pairs describing the body and the HTTP response 

### JSON
**described in RFC 4627** , as a standard for *representing* simple data structures in plain text:
- double quotes " " to represent **strings**
- square brackets [ ] to describe **lists**
- curly brackets { } to describe **objects**

### Collection+JSON

===**Content-Type: application/vnd.collection+json**===
*based on json* , is a standard for publishing a searchable list of resources over the
Web. Collection+JSON puts constraints on JSON , Because it can only serve json objects which in turns have a *collection* property which map to another object ,
the collection object must have and items property which map to a list of objects which represents HTTP resources with there href property.
so on and so forth you will get the highly formatted  collection+json document
**Collection+JSON is a way of serving lists that describe HTTP resources**  
the collection property have also a *href* property contain the URL that the client just sent request to it's the *address used to retrieve a representation of the document*
to submit data in the way html uses form to send data to the server , collection+json standard define the **template** property to send data as object in it

### HTTP POST: How Resources Are Born

POST is designed to allow a uniform method to cover the following functions:
-  Annotation of existing resources;
-  Posting a message to a bulletin board, newsgroup, mailing list, or similar group of articles;
-  Providing a block of data, such as the result of submitting a form, to a data-handling process;
- Extending a database through an append operation.

### Liberated By Constrains

**One counter intuitive lesson of RESTful design is that *constraints can be liberating*** 
for example The security constrains on the server enable us to send a GET request to any URL that we don't know what may it's representation look like and nothing terrible will happen. 
now if the server send a plain-text document that says 9, you can't tell if it's a number or a string it's completely ambiguous , in the other hand if it was a *json* document you that 9 is a number .
we conclude that *JSON put  more constrains* on the *meaning* of the document , as a result the server and the client can have a *meaningful conversation* .

when you make a new api that use JSON to Publish thing you have to specify how your API should look like , hundreds of APIs similliary use json but completely *incompatible* that's is **learning one API does't help a client learn the next one** .
for ex: Collection+Json standard provides more constrains so you don't have to explain what href property mean or what's the URL of and any *library* that understands collection+json format can use you API , So you *free* you self from writing a whole documentation and code and free your users from having to learn yet another API, as a Conclusion More Constrains less effort

### Application Semantics Create the Semantic Gap










## Resources and Representations

### A Resources Can Be Everything

