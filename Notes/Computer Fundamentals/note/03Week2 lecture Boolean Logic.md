# Week2 Lecture Boolean Logic

### Abstractions  

Abstraction is a technique for arranging complexity of computer systems  

### Top-down vs Bottom-up  

Waterfall development / Agile development

procedural / oop

Discrete event / Agents

### Building from Elementary Components  

build from millions of nano size transistors (used to build logic gate)

### Boolean Logic  

every chip can be built from AND OR NOT gate, and they can be built from NAND.

so: **every possible chip can be built from just the NAND gates**  

### Elementary Logic Gates  

![QQ截图20220927162325](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927162325.png)

### Gate Logic  

Gates with 3 or more inputs require composing a structure with
multiple gates (hence called composite gates)  

### The Super NAND  

![QQ截图20220927164526](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927164526.png)

### Boolean Expressions  

**precedence**

Parentheses > Not > And  > Or

### Laws of Boolean Algebra  

![QQ截图20220927172018](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927172018.png)

#### Idempotent law

 x Or x=x x And x=x

 x Or x Or x Or x ….. = x  

#### Associative law

(x Or y)Or z = x Or(y Or z)  

(x And y)z = x(y And z)  

#### Commutative law

x And y = y And x  

x Or y=y Or x  

#### Distributive law

 x and (y or z) =   (x and y) or (x and z)

x or (y and z) =  (x or y) and (x or z)  

#### De Morgans Law  

Not(x And y) = Not(x) Or Not(y)  

Not(x Or y) = Not(x) And Not(y)  

#### Complement law  

x And(Not(x))=0

x Or (Not(x))=1  

#### Double negative Law  

(NOT(NOT(x)))=x  

#### example1

Not(Not(x) And Not(x Or y))

= x OR (x OR y)

= (x OR x) OR y

= x OR y

### Boolean function synthesis  

from truth table to boolean function

![QQ截图20220927172812](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927172812.png)

### Multiplexers and Demultiplexers  

![QQ截图20220927174419](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927174419.png)

#### Multiplexer

![QQ截图20220927174608](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927174608.png)

#### Demultiplexer

![QQ截图20220927174616](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Computer Fundamentals (COMP1036 UNNC)\assets\QQ截图20220927174616.png)
