# Database
A database is an organized collection of data, generally stored and accessed electronically from a computer system.

The database management system (DBMS) is the software that interacts with end users, applications, and the database itself to capture and analyze the data. The DBMS software additionally encompasses the core facilities provided to administer the database.

DBMS often are classified according to the database models that they support. 

## [Seven Database Paradigms](https://fireship.io/lessons/top-seven-database-paradigms/)

1. Key-value
2. Wide Column
3. Document
4. Relational
5. Graph
6. Search Engine
7. Multi-model

### 1. Key-value
A key–value database, or key–value store, is a data storage paradigm designed for storing, retrieving, and managing associative arrays, and a data structure more commonly known today as a dictionary or hash table. 

Popular Databases: Redis, Memcached, Etcd

Pros:
- Very Fast

Cons:
- Limited space
- No Queries

Best For:
- Caching
- Pub/Sub
- Leaderboards

### 2. Wide Column
A wide-column store (or extensible record stores) is a type of NoSQL database. It uses tables, rows, and columns, but unlike a relational database, the names and format of the columns can vary from row to row in the same table. A wide-column store can be interpreted as a two-dimensional key–value store.

Popular Wide-Column Databases: Cassandra, Apache HBase

Pros:
- Schema-less
- Decentralized
- Scales horizontally

Cons:
- No Joins

Best For:
- Time-Series
- Historical Records
- High-Write, Low-Read

### 3. Document Oriented
A document-oriented database, or document store, is a computer program and data storage system designed for storing, retrieving and managing document-oriented information, also known as semi-structured data.

Document-oriented databases are one of the main categories of NoSQL databases.

Document-oriented databases are inherently a subclass of the key-value store, another NoSQL database concept. The difference lies in the way the data is processed; in a key-value store, the data is considered to be inherently opaque to the database, whereas a document-oriented system relies on internal structure in the document in order to extract metadata that the database engine uses for further optimization. Although the difference is often negligible due to tools in the systems, conceptually the document-store is designed to offer a richer experience with modern programming techniques.

Popular Document Databases: MongoDB, Firestore, CouchDB

Pros:
- Schema-less
- Relational-ish Queries
- Easy use

Cons: 
- Without joins

Best For:
- Most Apps
- Games
- IOT

### 4. Relational
A relational database is a digital database based on the relational model of data. A software system used to maintain relational databases is a relational database management system (RDBMS). Many relational database systems have an option of using the SQL (Structured Query Language) for querying and maintaining the database.

It uses a structure that allows us to identify and access data in relation to another piece of data in the database. Often, data in a relational database is organized into tables.

Popular Relational Databases: MySQL, Postgres, SQL Server, CockroachDB

Pros:
- Joins
- Queries
- ACID complient (atomicity, consistency, isolation, and durability)

Cons:
- Schema Required
- Dificult horizontal scaling

Best For:
- Most Apps

### 5. Graph
In computing, a graph database (GDB) is a database that uses graph structures for semantic queries with nodes, edges, and properties to represent and store data. A key concept of the system is the graph (or edge or relationship). The graph relates the data items in the store to a collection of nodes and edges, the edges representing the relationships between the nodes. The relationships allow data in the store to be linked together directly and, in many cases, retrieved with one operation. Graph databases hold the relationships between data as a priority. Querying relationships is fast because they are perpetually stored in the database. Relationships can be intuitively visualized using graph databases, making them useful for heavily inter-connected data.

Graph databases are a type of NoSQL database, created to address the limitations of relational databases. While the graph model explicitly lays out the dependencies between nodes of data, the relational model and other NoSQL database models link the data by implicit connections. In other words, relationships are a first-class citizen in a graph database and can be labelled, directed, and given properties. 

Popular Graph Databases: Neo4j, DGraph, Janus Graph

Pros:
- Fast queries
- Horizontal scaling

Best For:
- Heavily inter-connected data
- Graphs
- Knowledge graphs
- Recommendation Engines

### 6. Search Engine
A search-engine database is a type of nonrelational database that is dedicated to the search of data content. Search-engine databases use indexes to categorize the similar characteristics among data and facilitate search capability. Search-engine databases are optimized for dealing with data that may be long, semistructured, or unstructured, and they typically offer specialized methods such as full-text search, complex search expressions, and ranking of search results. 

Popular Search Databases: ElasticSearch, Algolia, MeiliSearch

Pros:
- Fast queries

Cons:
- Overhead
- Expensive to run at scale

Best for:
- Text search
- Logging and analysis

### 7. Multi-Model
In the field of database design, a multi-model database is a database management system designed to support multiple data models against a single, integrated backend. In contrast, most database management systems are organized around a single data model that determines how data can be organized, stored, and manipulated. Document, graph, relational, and key-value models are examples of data models that may be supported by a multi-model database.

Popular Multi-model Databases: FaunaDB, CosmosDB

Best for:
- Everything