# SQL1

### SQL and Database Management Systems (DBMS)

A DBMS is a collection of programs that enables users to create and

maintain a database, also provide interface for programming languages to interact with database.

Examples of DBMSs, include:

- SQLite

- MariaDB

- MySQL

### SQL

> Although SQL is a standard, it is not supported *exactly* the same way by all DBMSs.

#### SQL Sublanguages

- Data Definition Language (DDL)

- Data Manipulation Language (DML)

- Data Control Language (DCL)

### SQL CREATE

```sqlite
create table Student (
   ...> sID INTEGER not null primary key,
   ...> sNAME varchar(50) not null,
   ...> sAddress varchar(255),
   ...> sYear integer default 1
   ...> );
```

### Constrain

```sqlite
constrain pk_student primary key (SID)

sID Integer primary key

//have the same function
```

- **PRIMARY KEY** 

  • Primary keys cannot be NULL

  • Primary keys must be unique

  • Primary keys will typically add NOT NULL and UNIQUE constraints

- **UNIQUE** 

  • UNIQUE constraints can be NULL

  • UNIQUE constraints must be unique

  • This has the same effect as a primary key constraint, except that the column(s) can contain NULL values

  • This effectively creates a candidate key for the table

- NOT NULL

### Data Types

![QQ截图20221017094828](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20221017094828.png)

### Foreign keys

```sqlite
    FOREIGN KEY (mCode)
        REFERENCES Module (mCode)
```

**add referential integrity constrains** 

```sqlite
CONSTRAINT en_fk1
FOREIGN KEY (sID) REFERENCES Student(sID)
ON UPDATE CASCADE
ON DELETE CASCADE,
CONSTRAINT en_fk2
FOREIGN KEY (mCode) REFERENCES Module(mCode)
ON UPDATE CASCADE
ON DELETE CASCADE
```

- RESTRICT: The database will not allow the update or delete to proceed if it would break referential integrity

- CASCADE: The database will update/delete related rows in the other table
- SET NULL: The database will set the foreign key to NULL in the related row in the other table

> using
>
> ```sqlite
> PRAGMA foreign_keys = ON;
> ```
>
> to use foreign key constrains

### Deleting Tables (DROP)

```sqlite
DROP TABLE [IF EXISTS] table-name;

DROP TABLE IF EXISTS Student; # example
```

### SQLite Dot Commands

The most useful commands are:

- .help - Display a list of commands

- .tables - Display a list of tables

- .import - Import data from a file into a table

- .read - Execute commands from a file

- .schema - Display the schema of a table

- .quit - Exit the command line tool