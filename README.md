![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)

# NoSQL Research Lab

## Explainer

Up until now in the cohort we have stored data only in what are known as relational databases (SQL is the most well known type of relational DB querying language). Relational databases structure our data into tables. Today we will learn about a different type of database: a non-relational one. 

## Lab

In this lab you will be researching, either individually or in groups, answer to the following questions about noSQL databases. The intention is for you to spend some time learning about the fundamental differences between the type of databases we have seen before and the new type we will be learning about today. Even more importantly, you will learn about why two types of databases are used, and what situations fit each type of db. 

## Setup

Fork and clone this repository and answer questions as you research directly in the README. You do not have to submit this lab, but you will want to have it on hand for reference in the future. 

## Questions:

1. What does the term noSQL refer to, and what other term is often used synonymously with noSQL?
  - non-relational
  - does not use rows and columns
  - can be both tabular and non tabular

2. What are some of the common arguments for using a non-relational versus a relational db?
  - greater flexibility
  - greater scalability (in terms of changing data structure)
  - personal preference

3. In this class we will be using the document style of non-relational databases. What are the charecteristics of a document based db? 
  - json data (or json like data)
  - documents structure has fields/values -- values are a variety of support types
  - allows for the data model to evolve vs having a rigorous structure
  - no enforced schema

4. In this class we will be using Mongo specifically as our no-SQL db. Look into Mongo and answer this question: what is the priamry difference between how Mongo is maintained versus SQL?
  - mongo is open source, made by smaller company
  - some versions of SQL are closed source
    - Oracle, mySQL, microsoft SQL server
  - some version are open 
    - postgres, SQLite
  - one implementation to rule all of Mongo
    - same team makes all of the mongo tools
    - tight integration of all mongo features

5. Mongo DBs are organized into documents. Describe an example of a table in SQL that contains users, and then describe the equivalent DB setup in Mongo. 
  - user -> blog in SQL use either FK or join
  - mongo would have embedded objects or 'sub documents'
    - { userName, email, blogs: [{ blog }, { blog }] }

6. What is an example situation where a Mongo database makes sense versus a relational db?
  - fast paced development when the data models might change alot
  - adding features to the database
  - situations that involve collaborations between lots of teams

7. What are the benefits of SQL databases? NoSQL Databases?
  - Benefits of SQL:
    - commonality of language, lack of complex code
    - established and used in many places
  - Benefits of noSQL:
   - familiar languages to devs
   - 'data that is accessed together should be stored together'

8. Explain the differences between ACID and BASE models.
  - ACID
    - A: Transactions atomic
    - Consistent, ensures durability 
  - BASE: 
    - 'appears to work most of the time'
    - soft state (ie doesn't)

9. What should you consider when deciding between using a relational database or a non-relational database for your project?
 - personal preference
 - scale of traffic
 - speed
 - what kind of flexibility will you need


## Visual Comparisons

### Structure

![](https://media.git.generalassemb.ly/user/16103/files/65db7f00-afd5-11ea-926a-e51b2fd2be08)

### Relationships

![](https://media.git.generalassemb.ly/user/16103/files/5eb47100-afd5-11ea-8cae-0a65c924be4b)

### Use Cases

![](https://media.git.generalassemb.ly/user/16103/files/7f7cc680-afd5-11ea-82c8-10ed74ee2222)

## Additional Readings

Pick an additional reading to go through with a classmate. Reflect on how the
article changes the discussion. What have you learned?

  _**Note:** You do not have to read about the different types of SQL and NoSQL. We will use PostgreSQL and MongoDB in this course._
- [ACID vs. BASE Explained](https://neo4j.com/blog/acid-vs-base-consistency-models-explained/)
- [PostgreSQL Use Cases](https://www.cybertec-postgresql.com/en/postgresql-overview/solutions-who-uses-postgresql/)
- [MongoDB Use Cases](https://www.mongodb.com/use-cases)
- [What the heck are you actually using NoSQL for?](http://highscalability.com/blog/2010/12/6/what-the-heck-are-you-actually-using-nosql-for.html)
- [A co-Relational Model of Data for Large Shared Data Banks](http://queue.acm.org/detail.cfm?id=1961297&repost)
- [A brief history of databases](http://avant.org/media/history-of-databases)
- [NoSQL Databases: An Overview | ThoughtWorks](http://www.thoughtworks.com/insights/blog/nosql-databases-overview)
- [When to choose CouchDB vs RDBMS?](http://stackoverflow.com/a/2731207/402618)
- [CAP Twelve Years Later: How the "Rules" Have Changed](http://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed)
