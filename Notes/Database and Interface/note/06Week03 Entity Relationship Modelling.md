# Week03 Entity Relationship Modelling

### Relational Model and SQL

SQL is Based on the relational model
Tables, queries implements relational model and algebra  

### Database Design

Conceptual Design

- Build a model independent of the choice of DBMS  

### Entity/Relationship Model
![QQ截图20221010092449](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010092449.png)

#### Entities  

**Entities** represent objects or things of interest  

In E/R Diagrams, we will represent Entities as boxes with rounded corners  

#### Attributes  

**Attributes** are facts, aspects, properties, or details about an entity  

In an E/R Diagram attributes are drawn as ovals  

Each attribute is linked to its entity by a line  

#### Relationships  

**Relationships** are an association between two or more entities  

**Degree of Relationship**: the number of entities that participate  

**Relationship type** : an association between two or more entity types  

**Relationship instance** : a uniquely identifiable association that includes one instance from each participating entity type  

#### Cardinality Ratios  

Each entity in a relationship can participate in zero, one, or more than one instances of that relationship  

One to one (1:1)  

One to many (1:M)  

Many to many (M:M)  

![QQ截图20221010094642](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010094642.png)

### E/R Model vs Relational Model  

![QQ截图20221010094824](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010094824.png)

## How to draw E/R diagram

### Example

![QQ截图20221010100554](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010100554.png)

### find Entities  

department

course

modules

student

lecturer

### find Relationships

● A department offers several courses.
● A number of modules make up each course.
● Students enroll in a particular course.
● Students take several modules.
● Each module is taught by a lecturer.
● Each department employs a number of lecturers.
● Each lecturer tutors a group of students.  

### draw graph

![QQ截图20221010102946](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010102946.png)

### Removing M:M to 1:M

![QQ截图20221010103021](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010103021.png)

### Removing 1:1 to attributes

![QQ截图20221010103408](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221010103408.png)

### primary key

draw an underline under the attribute to identify the primary key

### Entities and Attributes  

- Entities can have attributes but attributes have no smaller parts

- Entities can have relationships between them, but an attribute belongs to a single entity  

