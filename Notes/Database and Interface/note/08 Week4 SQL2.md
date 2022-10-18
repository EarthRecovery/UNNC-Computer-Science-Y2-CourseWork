# SQL2

### INSERT Statement

```sqlite
INSERT INTO
table table_name (column1, ...)
VALUES
(value1, ...);
```

> if we don't give a value to primary key, DBM will auto give a primary key (always plus 1).

```sqlite
insert into student values (null,'LLL','China',1);

insert into Student(sNAME, sAddress, sYear)
values ('xxx','China',2);

-- have the same function
```



### (Simplified) SELECT Syntax

```sqlite
SELECT
	column1, ...
FROM
	table_name
WHERE
	condition;
ORDER BY
	column1, ... ASC|DESC;
GROUP BY
	column1, ...
HAVING
	condition
```

> ASC is an optional keyword that tells SQL to sort in ascending order (default)
>
> DESC is an optional keyword that tells SQL to sort in descending order

