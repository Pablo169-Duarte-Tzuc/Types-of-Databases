<h1><center>Document, Ledger and Search Databases</center></h1>

<p align="center">
  <img src="https://community-cdn-digitalocean-com.global.ssl.fastly.net/assets/tutorials/images/large/Database-Mostov_v4.1_twitter-_-facebook.png?1546896970?raw=true" alt="Sublime's custom image"/>
</p>



## Preface
We recently had a video conference with a friend of our professor Juan vazquez named Paco Ocampo, Paco is a person who knows about managing the cloud for big data and this time he told us about the different types of databases that we can find in the google cloud.

Although databases are essential today for any public and private company, why? This is due to the fact that they are more efficient when storing information (without papers) and less contamination, but without a doubt one of their main advantages of using them is the great value that we can obtain from them, as we usually hear "When life hands you lemons, make lemonade. ", with the data we can even predict the future.

But if you want to know about databases you can search for pages, documents, books among other types of resources, that is why in this document we will focus on the three different types of databases that currently exist (Document, Ledger and Search), we hope you like it .


## Document databases

This type of database is built similar to a JSON file,
XML & YAML or binary formats such as BSON so if we have knowledge of this type of document either because we program in JavaScript or use them to build data frames in python with the help of pandas.

> Here is an example of what the format would look like:

![ejemplo1](https://webassets.mongodb.com/_com_assets/cms/Code%20Snippet%20545%20x%20330@4x-zgzlrug0va.png)


This type is one of the most popular alternatives that can be used as rational tabular databases and according to Wikipedia they constitute one of the main subcategories within the so-called NoSQL databases.

Some characteristics that we will talk about later are the following:

> Natural and flexible 

> They promise higher developer productivity, and faster evolution with application needs.

Here some examples of systems of Document Databases

![imagen3](https://www.practicalecommerce.com/wp-content/uploads/2016/07/070116-nosql-db-570x276.png)


# Different between relational databases

## Intuitive data model:
> The documents are assigned to the objects in the code, this makes it easier to work with them.

> As shown in the first image, the structure of this database is different from a DB SQL, therefore we will not need to execute "joins" that consume a lot of resources.

> We can put the data together or as pipes, this allows us to write less code and gives us more performance for queries.

## Flexible Scheme:
> The documents are dynamic, this means that it is not necessary to define them previously in the DB.

> The fields of the documents can vary, and the structures can be modified at the moment we want, allowing us to avoid disruptive schema migrations.

## Powerful:
> Ad hoc queries, indexing, and real-time aggregations provide powerful ways to access, transform, and analyze your data.

> With the help of ACID transactions, the same guarantees are maintained as a DB SQL, that is, we can manipulate data from a single document or multiple documents that live in multiple fragments.

## The Distribution:
> These databases are systems distributed at their core, so each document is independent of another, this provides us with an ease when it comes to distributing them on various servers.

> According to the document DB mongo dB page, native fragmentation provides an elastic and transparent horizontal scale to the application to accommodate the growth of its workload, along with geographic data distribution for data sovereignty.

## Graphical difference between a relational database and one based on documents

![imagen4](https://webassets.mongodb.com/_com_assets/cms/Relational_vs_DocumentDB-imgngssl17.png)


## Ledger Database.
### Why “ledger”?

The term ledger represents the way we used to record information before computers. Before computers, we recorded information in books, sometimes called ledgers, where data was only appended and you could view the past. In the early years of computers, hardware was expensive. Thus we built systems that update in place and use the most efficient amount of memory. Now that we’re in the age of cheap, commodity hardware, we can revert to recording information in a more intuitive and useful way.

*"Ledger Database — A NoSQL database that provides an immutable, transparent, and cryptographically verifiable transaction log •owned by a central authority. — Amazon’s QLDB Overview"*

*"A non ledger database is table-centric. A ledger database is log-centric. The log is the database."*

To begin with:
* it is not a NoSQL database (usually)
This is different from the usually NoSQL database we're getting, it's different form Microsoft SQL Server, Oracle, MYSQL servers.
Data is stored as a document without and natural relationships to other documents, but in this case this works as a relational database. 
* It is immutable.
In ledger databases, these can never been changed. So no matter what changes happen you will never overwrite the existing data. 
* It is trasnparent.
It's the ability to see the changes to records and data over time. 
* It is cryptographically verified.
This mean that the records or data are hashed. In a simple way the long string of data that is the record is paired down to a much smaller string of characters that is unique. 

### How does work it?
Let's suppose that we create an order:
![ex1](https://ivan.mw/images/ledger-1.jpg)
Then We update it.
![ex2](https://ivan.mw/images/ledger-2.jpg)
Then we do update it again
![ex3](https://ivan.mw/images/ledger-3.jpg)

The key insight is that ledger databases remember the past. New information doesn’t overwrite the past but is instead added to it. The log is the heart of the database and the source of truth, not the tables. Each update is appended to the log as a new entry.
### Example of legder based architecture
![ex4](https://ivan.mw/images/ledger-4.jpg)

The ledger database contains the log and tables which are a view into the log’s data. In this case, I have an Orders table which shows the latest status of each order. That same log data is fed into an email system, which emails customers updates on their orders, a billing system, which filters through log data and tracks each CREATED order, and a data warehouse, which is used to run analytics on the data.

# Search Databases 
![imagen6](https://discoversdkcdn.azureedge.net/postscontent/elastic_solr.jpg)

Search engines are NoSQL database management systems dedicated to searching for data content. In addition to general optimization for this type of application, specialization typically consists of offering the following features:

* Support for complex search expressions
* Full-text search
* Stemming (reducing inflected words to their root)
* Sorting and grouping search results
* Geospatial search
* Distributed search for high scalability

# Important examples
* Elasticsearch
* Splunk
* Solr
* MarkLogic
* Sphinx


The databases use different search engines identified by the companies that provide access to them.They are simple and intuitive search interfaces, aimed at all types of users, which usually have two search modes: simple and advanced.

Examples of the most used search engines:
> Ebsco

> Proquest

> Ovid.


## Matrix 
| Criteria and Example  | Big Query                                                                              | Elastic Search                                                                                                                                                                                                                                                                                                                                                                     | MongoDB                                                                                                                                                                                                                                                                                                                                                                                            | CouchDB                                                                                                                                                                                                                           | Amazon QLDB                                                                                                                                                                                                                                           | Big ChainDB                                                                                                                                                                                                                                                                                                                       |
|-----------------------|----------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Database Type         | Search                                                                                 | Search                                                                                                                                                                                                                                                                                                                                                                             | Document                                                                                                                                                                                                                                                                                                                                                                                           | Document                                                                                                                                                                                                                          | Ledger Data Base                                                                                                                                                                                                                                      | Ledger Data Base                                                                                                                                                                                                                                                                                                                  |
| Authors(Developers)   | Google                                                                                 | Elastic, Shay Banon                                                                                                                                                                                                                                                                                                                                                                | MongoDB Inc.                                                                                                                                                                                                                                                                                                                                                                                       | Damien Katz                                                                                                                                                                                                                       | Amazon Web Service                                                                                                                                                                                                                                    | BigchainDB                                                                                                                                                                                                                                                                                                                        |
| Best Used             | Cost control<br>Dynamic permission control<br>Linking sheets                           | Search for applications <br>Website search <br>Business Search<br>Logging and log analytics<br>Infrastructure metrics and container monitoring<br>Application performance monitoring <br>Geospatial data analysis and visualization<br>Security analytics<br>Business Analytics                                                                                                    | Event storage and log<br>Document and content management systems<br>Electronic commerce<br>Games<br>Systems with high volume of readings<br>Mobile apps<br>Website operational data warehouse                                                                                                                                                                                                      | For accumulating, occasionally changing data, on which pre-defined queries are to be run. <br>Places where versioning is important.                                                                                               | With QLDB you can match system log applications, those whose data integrity, integrity, and verifiability are critical. As an example in economics, critical monitoring data from registry system applications such as credit and debit transactions. | BigchainDB is for developers and organizations looking for a queryable database with blockchain characteristics such as decentralization, immutability and the ability to treat anything stored in the database as an asset. Whether it’s atoms, bits or bytes of value, any real-world blockchain application needs performance. |
| Usage Example         | Retail and consumer goods                                                              | It is excellent at full-text search.<br>Elasticsearch is  a near real-time search platform, which implies that the latency between the moment a document is indexed until the moment it can be searched is very short: typically, one second.<br>As a result, Elasticsearch is well prepared for time-constrained use cases like security analytics and infrastructure monitoring. | To do similar things with mySQL or postgreSQL but with greater speed and comfort                                                                                                                                                                                                                                                                                                                   | CRM, CMS systems.<br> Master-master replication is an especially interesting feature, allowing easy multi-site deployments.                                                                                                       | Designed for organizations that want to keep a verifiable and encrypted history of information changes in an application they own, such as accounting systems, bank transfer systems, credit card transaction system, among others.                   | Decentralization: No single point of control <br>Query: Running any MongoDB query for transactions,assets,metadata and blocks. <br> Low latency: Use for fast velocity<br> Rich Permissioning: Set permissions at transation level <br> Purblic or Private                                                                        |
| Known Shortcomings    | Linking sheets                                                                         |                                                                                                                                                                                                                                                                                                                                                                                    | It can't make transactions Doesn't have a replacement for inheritance solutions.                                                                                                                                                                                                                                                                                                                   | Slower than in-memory DBMS.<br>In-place updates require server-side logic (update handlers).<br>Temporary views on large datasets are very slow.                                                                                  | For each AWS service. Unless we indicate otherwise, each quota or limit is specific to the region.Not in all regions is available                                                                                                                     |                                                                                                                                                                                                                                                                                                                                   |
| Main Focus            | Designed for analyzing data on the order of billions of rows, using a SQL-like syntax. | Search and analytics engine that centrally stores your data so you can search, index, and analyze data of all shapes and sizes                                                                                                                                                                                                                                                     | Have some familiarities with SQL in querying and indexing                                                                                                                                                                                                                                                                                                                                          | DB Concistency and easy use.                                                                                                                                                                                                      | Fully managed ledger database providing a transparent, immutable, and verifiable transaction log using cryptography. Owned by a central trusted authority.                                                                                            | Big data distributed database and then adds blockchain characteristics - decentralized control, immutability and the transfer of digital assets.                                                                                                                                                                                  |
| License               | Google                                                                                 | Apache                                                                                                                                                                                                                                                                                                                                                                             | AGPL (Drivers: Apache)                                                                                                                                                                                                                                                                                                                                                                             | Apache                                                                                                                                                                                                                            | Amazon                                                                                                                                                                                                                                                | Apache                                                                                                                                                                                                                                                                                                                            |
| Pricing               | Scalable Price                                                                         | Scalable Price                                                                                                                                                                                                                                                                                                                                                                     | You can use it for free or pay for instances + mongolab                                                                                                                                                                                                                                                                                                                                            | Open Source                                                                                                                                                                                                                       | Scalable Price                                                                                                                                                                                                                                        | Open Source                                                                                                                                                                                                                                                                                                                       |
| Projects Using it     | Safari Books Online uses BigQuery for Business Intelligence                            | InfoTrack - Potenciar la búsqueda de innovación impulsada por datos con Elasticsearch Service                                                                                                                                                                                                                                                                                      | Square Enix - editor of games has issues with the scalability limits of relational databases<br>before it migrated to MongoDB.<br><br>The city of Chicago develops a smart <br>platform (WindyGrid) with the help of mongodb<br><br>The Washington Post built a content tool that <br>uses MongoDB to help a diverse group of teams <br>create dynamic forms and <br>responses to articles online. | CouchDB is used in certain Android applications, such as "SpreadLyrics"<br>Facebook applications like "Will you Kissme" or "Birthday Greeting Cards"<br>Ubuntu used couchDB for its "Ubuntu One" sync service until November 2011 | Humboldt uses QLDB to help preserve tropical forests in Brazil.                                                                                                                                                                                       | Own the Music You Stream with Resonate“Every Product Has a Story” - innogy’s Digital Product MemoryVerified Educational Credentials with Recruit TechnologiesBlockchain Powered Land Registry in Ghana with BenBen                                                                                                                |
| Latest Version        |                                                                                        | 5.4                                                                                                                                                                                                                                                                                                                                                                                | 4.2                                                                                                                                                                                                                                                                                                                                                                                                | 3.1.0                                                                                                                                                                                                                             | API version: 2019-01-02                                                                                                                                                                                                                               | 2.0                                                                                                                                                                                                                                                                                                                               |
| Data Presentation     | JSON                                                                                   | JSON                                                                                                                                                                                                                                                                                                                                                                               | JSON                                                                                                                                                                                                                                                                                                                                                                                               | JSON                                                                                                                                                                                                                              | like ledgers                                                                                                                                                                                                                                          | JSON                                                                                                                                                                                                                                                                                                                              |
| Development Language  |                                                                                        | JAVA                                                                                                                                                                                                                                                                                                                                                                               | C++                                                                                                                                                                                                                                                                                                                                                                                                | Erlang                                                                                                                                                                                                                            |                                                                                                                                                                                                                                                       | Python Driver<br>JavaScript / Node.js Driver<br>Java Driver                                                                                                                                                                                                                                                                       |
| Platforms             | Cloud                                                                                  | CROSS-PLATAFORM                                                                                                                                                                                                                                                                                                                                                                    | CROSS-PLATFORM                                                                                                                                                                                                                                                                                                                                                                                     | Cross-platform                                                                                                                                                                                                                    | Cross-platform                                                                                                                                                                                                                                        | Cross-Plattform                                                                                                                                                                                                                                                                                                                   |
| Protocol              | RPC-Based                                                                              | HTTP                                                                                                                                                                                                                                                                                                                                                                               | BSON (Binary)                                                                                                                                                                                                                                                                                                                                                                                      | HTTP/RES                                                                                                                                                                                                                          | HTTP                                                                                                                                                                                                                                                  | CrThe HTTP Client-Server API<br>The WebSocket Event Stream API                                                                                                                                                                                                                                                                    |
| Website               | https://cloud.google.com/bigquery                                                      | https://www.elastic.co/es/                                                                                                                                                                                                                                                                                                                                                         | https://www.mongodb.com/                                                                                                                                                                                                                                                                                                                                                                           | https://www.couchbase.com/                                                                                                                                                                                                        | https://aws.amazon.com/es/qldb/                                                                                                                                                                                                                       | https://www.bigchaindb.com/                                                                                                                                                                                                                                                                                                       |


**References:**
* https://ivan.mw/2019-11-24/what-is-a-ledger-database
* https://hackernoon.com/relational-nosql-ledger-databases-work-not-permissioned-blockchains-9ccaef7b3139
* https://medium.com/a-technologists-pov/do-i-need-a-ledger-database-what-is-it-6f3b7261238
* https://platzi.com/tutoriales/1566-bd/2282-que-tipos-de-base-de-datos-existes-actualmente/
* http://rcientificas.uninorte.edu.co/index.php/salud/article/viewArticle/3822/5744
* https://aws.amazon.com/es/qldb/faqs/
* https://docs.aws.amazon.com/qldb/latest/developerguide/document-history.html
* https://www.mongodb.com/document-databases
* https://en.wikipedia.org/wiki/Document-oriented_database



