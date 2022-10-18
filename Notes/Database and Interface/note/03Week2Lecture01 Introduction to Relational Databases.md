# Week2 Lecture01 Introduction to Relational Databases  

**what is a database?**

- A collection of data
- A structured set of data
- using to update and select data

CRUD : )

### structure

![QQ截图20220926091203](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926091203.png)

SQL(Structured query language) - > data definition, manipulation, query

### DMBS

- sql
- sqlite
- DB2
- Oracle

### ANSI/SPARC Model  

American National Standards Institute  

Standards Planning Requirements
Committee  

**three layers of Database System**

![QQ截图20220926091755](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926091755.png)



**Internal Level**

○ Defines how data is stored in the database (storage space allocation, data structures, indexing, data compression, encryption, etc.)
○ Used by System designers  

**Conceptual (Middle) Level**  

○ Defines what data is stored in the database and the relationships between
data (e.g., table definitions, constraints on the data, security and integrity information)
○ Deals with the organization of the entire database content
○ Database Administrator  

**External**

○ Defines the user’s view of the database (the part of the database that is relevant to each user)
■ Based on the user’s interests,
● E.g., YY/MM/DD,
DD/MM/YYYY
■ Used by users and applications programmers  

### Relational Model  

**Relational Data Structure**  

Data is stored in relations which are tables with columns and rows  

(a relation is a set of tuples)

![QQ截图20220926092431](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926092431.png)

> domain of name->varchar(20)

**Named and Unnamed Tuples**  

**named:**

{ (Name, John), (Age, 23) }  

**unnamed:**

(John, 23) (equivalent to the above)  

> There is no real difference between named and unnamed tuples, but be
> careful with the ordering of unnamed tuples  

**Tuples of the graph** (named schema)

{ { (Name, John), (Age, 23) },
{ (Name, Mary), (Age, 20) },
{ (Name, Mark), (Age, 18) },
{ (Name, Jane), (Age, 21) } }  

**Degree and Cardinality**

Degree of a relation: how long is the tuple

Cardinality of a relation: haw many tuples exists

**example:**

![QQ截图20220926093158](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926093158.png)

### Properties of Relations  

• Each cell contains exactly one single value.
• Each attribute has a distinct name.
• The values of an attribute are all from the same domain.
• Each tuple is distinct, i.e., no duplicate tuples.
• The order of attributes has no significance.
• The order of tuples has no significance either  

### Candidate Keys  

A candidate key is a single field or the least combination of fields that uniquely identifies each record in the table  

● Every tuple has a unique value for that set of attributes: **uniqueness**
● No proper subset of the set has the uniqueness property: **minimality**  **(Superkey)**

> 超键：在关系中能唯一标识元组的属性集称为关系模式的超键。 注定义中的“属性集”，超键可以是一个很大的集合，只要他能确定是哪一行就行，因此’id’,‘user’,‘pwd’,‘section’,'name’都可以是超键的集。
>
> 候选键：不含有多余属性的超键，比如在上面的超键中，'id’自己就可以独自确定是哪一行，所以他自己可以是一个候选键，除去它以外的另外四个也可以是候选键，但是这五个放在一起因为有了多余的列，他们就不是候选键。（另外四个可以是候选键的原因是每一列都有可能有重复的内容）
>
> 主键：在所有的候选键里面找一个作为主键供使用，也就是说可以是id，也可以是另外四个的合体，也有可能是其他的选择，只要能保证选择的集合能唯一确定即可。

### Primary Keys  

One candidate key is usually chosen to identify tuples in a relation, which is primary key

###  NULLs  

- Missing information can be represented using NULLs  

- primary key can't have NULL

### Foreign Keys  

Foreign Keys are used to link data in two relations.  

**examples**

![QQ截图20220926094734](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926094734.png)

### Referential Integrity  (foreign key constrain)

##### RESTRICT

RESTRICT stops any action that violates integrity  

##### CASCADE

CASCADE allows the changes made to flow through  

##### SET NULL

SET NULL allows the changes to happen  but every attribute effected will become null (only foreign key)

> ![QQ截图20220926095428](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926095428.png)