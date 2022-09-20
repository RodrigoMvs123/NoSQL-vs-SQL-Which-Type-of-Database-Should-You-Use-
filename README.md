# NoSQL-vs-SQL-Which-Type-of-Database-Should-You-Use-

https://www.youtube.com/watch?v=FzlpwoeSrE0

##
https://raw.githubusercontent.com/RodrigoMvs123/NoSQL-vs-SQL-Which-Type-of-Database-Should-You-Use-/main/README.md
##
https://github.com/RodrigoMvs123/NoSQL-vs-SQL-Which-Type-of-Database-Should-You-Use-/blame/main/README.md
##

NoSQL vs SQL – Which Type of Database Should You Use?


https://www.youtube.com/watch?v=FzlpwoeSrE0

What actually is a Database?
Database design 
What is a Database Management System?
Relational Database
SQL
Non-relational Databases
SQL vs NoSQL
Pros and Cons
Use-cases
NoSQL Crash Course 

https://www.datastax.com/

Small Digital Storage
SD Card
Hard Drive
USB

Large Digital Storage 
Computer Cluster 
Cloud Storage 

File System / Desktop / Course Work / Personal Files
Hard Drive
Computer Cluster 

Hierarchical Database Model
Network Model
Relational Model
Entity-relationship Model
Enhanced entity-relationship Model
Object Model
Document Model
Tabular/ Wide-Column Type
Key-value Model
Entity-attribute-value Model
Star Schema
Inverted Index
Flat File
Correlational Model
Multidimensional Model
Multi-value Model
Semantic Model
XML Database
Property Graph 
Triplestore 

Relational / Wide-column / Document / Key-Value ( https://www.datastax.com/ )

Get Data / Add Data / Delete Data / Update Data 

Our Fingers / DBMS / Data

Some DBMS
SolarWinds Database Performance Analyzer 
Dbvisualizer 
ManageEngine Applications Manager 
Oracle RDBMS
IBM DB2
Microsoft SQL Server
SAP Sybase ASE
Teradata
ADABAS
MySQL
FileMaker
Microsoft Access
Informix
SQLite
PostgresSQL
AmazonRDS
MongoDB
CouchDB
Neo4j
OrientDB
Couchbase
Toad
Datastax Astra
phpMyAdmin 
SQL Developer
Seqel PRO
Robomongo
Hadoop HDFS
Cloudera
MariaDB
Informix Dynamic Server
4D (4th Dimension)
Altibase
Redis

Datastax 
Create Databse
CQL Console 

Relational Databases / Related Tables 
MySQL
MariaDB
PostgreSQL
Users/ Tags / Movies / Ratings 

Create Table student_grades (
    id int,
    name varchar ( 255 ),
    math varchar ( 255 ),
    art varchar ( 255 ),
    geography varchar ( 255 ),
PRIMARY KEY ( id ) 
);

INSERT INTO student_grades (
id, name, math, art, geography 
) VALUES ( val1, val2, val3, val4, val5 );


INSERT INTO student_grades (
id, name, math, art, geography 
) VALUES ( “013s3”, “Xiun”, “10/10”, “8/10”, “6/10” );


SELECT * FROM student_grades;


https://www.db-fiddle.com/



    {
  "clientID": "ejZSLDRAyoNWHuTOWdNCOzXX"
  "clientSecret": "sIiyRyz9Fyxz5joJ8v0yFpBNrw8sHkYTmqZmf-X1Rbhrdd0k2IxX8lMW4raROBpB7kzn54Z0O2HSHeDyEY932WMxXPAZi+EfxxmWWT62RD7_ga2KznN8JEo.jfm4_c7q"
  "token": "AstraCS:ejZSLDRAyoNWHuTOWdNCOzXX:3fe2750d8a2149473df2106520a413b4c985a407efd28565bfe71dab173e5ae4"
}

)

Non-Relational Databases
wide-column / document / key-value 
NoSQL Databases 

Wide-column Database tutorial 
 https://www.datastax.com/
   {
  "clientID": "ejZSLDRAyoNWHuTOWdNCOzXX"
  "clientSecret": "sIiyRyz9Fyxz5joJ8v0yFpBNrw8sHkYTmqZmf-X1Rbhrdd0k2IxX8lMW4raROBpB7kzn54Z0O2HSHeDyEY932WMxXPAZi+EfxxmWWT62RD7_ga2KznN8JEo.jfm4_c7q"
  "token": "AstraCS:ejZSLDRAyoNWHuTOWdNCOzXX:3fe2750d8a2149473df2106520a413b4c985a407efd28565bfe71dab173e5ae4"
}

CQL Console 
token@cqlsh >Show host
token@cqlsh >show version;
token@cqlsh >DESC KEYSPACES;
token@cqlsh >USE wide_column;
token@cqlsh:wide_column> CREATE TABLE IF NOT EXISTS pizzas (
… pizza_id UUID, 
… brand TEXT, 
… name TEXT, 
… ingredientes SET <TEXT>, 
… PRIMARY KEY (pizza_id));
 token@cqlsh:wide_column> DESC KEYSPACE wide_column;
token@cqlsh:wide_column> INSERT INTO pizzas (pizza_id, brand, name, ingredientes)
… VALUES ( uuid(), ‘Oetkers’, ‘Pineapple Pizza’, { ‘pineapple’, ‘cheese’, ‘ham’});
token@cqlsh:wide_column> SELECT * FROM pizzas; 
token@cqlsh:wide_column> INSERT INTO pizzas (pizza_id, brand, name, ingredientes)
… VALUES ( uuid(), ‘Pizza Hut’, ‘BBQ Pizza’, { ‘Beef’, ‘cheese’, ‘BBQ sauce’});
token@cqlsh:wide_column> SELECT * FROM pizzas; 
token@cqlsh:wide_column> INSERT INTO pizzas (pizza_id, brand, name, ingredientes)
… VALUES ( uuid(), ‘Ristorante’, ‘Broccoli Pizza’, { Broccoli’, 'Mozzarella', ‘Corn’});
token@cqlsh:wide_column> SELECT * FROM pizzas; 
… where pizza_id = // unique identifier; ( Pizza Id ) 
 
 token@cqlsh:wide_column> 
Document Database

 https://www.datastax.com/
Add Database Keyspace 
Connect 
Launching Swagger UI 
Post 
Try it out 
Token Management 
AstraCS:QJzRUfshWHxkmZeZLZXNwiZA:614603e3d6f841dd8a43bfbad16cb51eb358e5832851b3132f1a3cb2e986878a

The JSON Document 
Edit value Model

{
“name” : “cauliflower pizza” 
} 
Click Execute  ( Document ID //2 ) 

{
“name” : "mozzarella pizza” 
“calories” : 200
}
Click Execute 
GET 
Execute 


Key-value Database 
 https://www.datastax.com/
Add Keyspace 
Tutorial 
Add Keyspace Database 
Key_value 
Click Save 
Connect 
GraphQL API 
Launching GraphQL Playground 


mutation {
   createTable (
   KeyspaceName : "key_value",
   tableName: "pizzas",
   partitionKeys: [{name: "pizza_id", type: {basic: UUIU}}],
   values: [
       {name: "name", type: {basic: TEXT}},
       {name: "brand", type: {basic: TEXT}},

   ]
   )
}


{
    "data": {
        "createTable" : true 
    }
}

End Point graphql-schema 	/   graphql/key_value 


mutation {
   createTable (
   KeyspaceName : "key_value",
   tableName: "pizzas",
   partitionKeys: [{name: "pizza_id", type: {basic: UUIU}}],
   values: [
       {name: "name", type: {basic: TEXT}},
       {name: "brand", type: {basic: TEXT}},

   ]
   )
}


{
    "data": {
        "createTable" : true 
    }
}


End Point graphql-schema 	/   graphql/key_value 

mutation {
    insertpizzas (
        value: {
        pizza_id: "AstraCS:QJzRUfshWHxkmZeZLZXNwiZA:614603e3d6f841dd8a43bfbad16cb51eb358e5832851b3132f1a3cb2e986878a , name: pineapple pizza", brand: "dominos"
        }
    ) {
        value {
            pizza_id, name, brand 
        }
    }
}

mutation {
    updatepizzas (
        value : {
            pizza_id: "AstraCS:QJzRUfshWHxkmZeZLZXNwiZA:614603e3d6f841dd8a43bfbad16cb51eb358e5832851b3132f1a3cb2e986878a"
            name: "Watermelon Pizza", 
            brand: "dominos"

        }
    ) {
        value{
            pizza_id,
            name,
            brand
        }
    }
}

 

mutation {
    deletepizzas (value: 
    {pizza_id: "3683-wij3-id3j2-dpdq"
    }) {
    value {
        pizza_id
    }
    }
}


query {
    pizzas (value: {pizza_id: "3683-wij3-id3j2-dpdq" }
    ) {
        values {
            name,
            brand,
            pizza_id
        }
    }  
}


mutation {
    insertpizzas (
        value: {
            pizza_id "3683-wij3-id3j2-dpdq",
            name: "chocolote pizza", 
            brand: "Lindt"
        }
    ) {
        value {
            pizza_id,
            name,
            brand       
        }
    }
}


https://www.datastax.com/
token@cqlsh > CQL Console 
token@cqlsh > DESC keyspaces,
token@cqlsh > Use key_value ;
token@cqlsh:key_value > DESC key_value;
token@cqlsh:key_value >
datastax_sla / document / wide-column / system_views
…
token@cqlsh:key_value > SELECT * FROM pizzas;
token@cqlsh:key_value >


https://stargate.io/
