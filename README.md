Database is a collection of related data and data is a collection of facts and figures that can be processed to produce information.

ACID - 
A - Atomicity - entire tnx takes place at once or doen't happen
C - Consistency - Database must be consitenet before and after the tnx
I - Isolation -  Multiple tnx occurs concurrently without any interference
D - Durability - The changes of a successful tnx occurs even if the sys failures occurs

DBMS Architecture:
Can be centralised, decentalised or hierarchical.
1 tier Architecture: Only DBMS is there. Mostly used by programmers
2 tier architecture: Database and application layer is there which fetch data from the DB.
3 tier Architecture: Database,Application(middle layer) and end user. 

![image](https://github.com/rrairajeev/SQL/assets/169693667/6c3e2437-877b-49d4-a248-1f3da2fc4de7)

## DATA MODELS
Data models define how the logical structure of a database is modeled. Data models define how data is connected to each other and how they are processed and stored inside the system.

## ER Model
Entity Relationship Model
Eg. In a school, student is entity and name,age etc are attributes which has values.
Connection b/w entities are called relationships.
It can be one on one, one to many, many to many, many to one.


## Relational Model
The most popular data model in DBMS is the Relational Model. It is more scientific a model than others. This model is based on first-order predicate logic and defines a table as an n-ary relation.

![image](https://github.com/rrairajeev/SQL/assets/169693667/93dcd07a-c0c4-45db-8af4-c70ed2a4882d)

* Data is stored in tables called relations.
* Relations can be normalized.
* In normalized relations, values saved are atomic values.
* Each row in a relation contains a unique value.
* Each column in a relation contains values from a same domain.


## Database Instance
A database instance is a state of operational database with data at any given time. It contains a snapshot of the database. Database instances tend to change with time. A DBMS ensures that its every instance (state) is in a valid state, by diligently following all the validations, constraints, and conditions that the database designers have imposed.


## Database Schema
It is important that we distinguish these two terms individually. Database schema is the skeleton of database. It is designed when the database doesn't exist at all. Once the database is operational, it is very difficult to make any changes to it. A database schema does not contain any data or information.
Physical Schema: How data is store in seconday layer
Logical schema: This schema defines all the logical constraints that need to be applied on the data stored. It defines tables, views, and integrity constraints.


## Data independence

Metadata -  Data about data 
eg. where the data is, when changed etc.

Metadata itself follows a layed architecture so that when data is changed at one layer it doesn't affect the other layers.
Data is independent but mapped to each other. 

## Logical Data independence: 
Logical data is data about database, that is, it stores information about how data is managed inside. For example, a table (relation) stored in the database and all its constraints, applied on that relation.

## Physical Data Independence
All the schemas are logical, and the actual data is stored in bit format on the disk. Physical data independence is the power to change the physical data without impacting the schema or logical data.
eg. in case we want to change or upgrade the storage system itself − suppose we want to replace hard-disks with SSD − it should not have any impact on the logical data or schemas.
