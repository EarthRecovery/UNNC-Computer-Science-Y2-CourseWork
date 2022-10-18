# Week2Lecture02 Relational Algebra

### What is relational algebra

English <-> Relational Algebra <->SQL queries  

### Relations: mathematical definition  

A relation R of degree n, where values come from domains A1, …, An:
$$
R ⊆ A1 × A2 × … × An
$$
subset of the **Cartesian product of domains**  

## Unary Operators  

**example**

![QQ截图20220926101113](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926101113.png)

### Selection  

• 𝜎: selection operator
• 𝛼: properties
• R: target relation  

𝜎_𝛼(𝑅) = {(𝑎1, … , 𝑎𝑛) | (𝑎1, … , 𝑎𝑛) ∈ 𝑅, 𝛼(𝑎1, … , 𝑎𝑛)}

**example**

![QQ截图20220926101916](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926101916.png)

```sql
select * from Student where GPA>19
```

```sql
select * from Student where GPA>19 and HS<1000
```

```sql
select * from Apply where uName='Notts' and Subj='CS'
```

```sql
select * from (select * from Apply where uName='Notts') where Subj='CS'
```

### Projection  

Projection works as slicing  

• Projection of R on 𝑋 is represented as:
$$
𝜋_𝑋 (𝑅)
$$
• 𝜋: projection operator
• X: a set of attributes
• R: target relation
• 𝜋𝑋 𝑅 is a new relation only contain attributes from X  

**example**

![QQ截图20220926102309](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926102309.png)

```sql
select SID,Dec from Apply
```

```sql
select SID,sName from (select * from Student where GPA>19)
```

## Set Operators  

### Union

![QQ截图20220926102833](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926102833.png)

### Set difference  

![QQ截图20220926103024](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926103024.png)

### Intersection  

![QQ截图20220926103132](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926103132.png)

### Cartesian product  

![QQ截图20220926103218](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926103218.png)

## Joint Operators  

### Natural Join Operator  

Same as Cartesian Product but enforces equality on all attributes with the same name (S.SID and A.SID in our case)  

##### ![QQ截图20220926104027](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926104027.png)

**example**

![QQ截图20220926104116](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926104116.png)

**if two graph do not have the common attribute, Natural joint will have the same as the Cartesian joint**

### Theta Join Operator  

![QQ截图20220926104539](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926104539.png)

### Rename Operation

![QQ截图20220926104653](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Databases and Interfaces (COMP1048 UNNC)\assets\QQ截图20220926104653.png)