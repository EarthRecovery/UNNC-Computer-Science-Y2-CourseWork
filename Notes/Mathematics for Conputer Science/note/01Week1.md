# Week1

> section 1.4 and 1.5

propositions:

predicates: a property that the subject of a statement can have.

using p(x) to annotate

once the variable x has been assigned, the statement P(x) becomes a proposition

when we have multiple variables, called P(x1,x2,x3...xn)

### Quantification

- universal : "all" whether is always true
- existential : "some" one or more elements is true

**P(x) for all valuables of x is in the domain**
$$
\forall xP(x)
$$
true if all the domain of x makes P(x) true

**Existential quantifier**
$$
\exists xP(x)
$$
true if some of x make P(x) true

### Restricted domain

$$
\forall x < 0 (x^2>0) == \forall x(x<0 \longrightarrow x^2>0)
$$

$$
\exist z>0 (z^2>0) == \exist z(z  > 0 \longrightarrow z^2 = 2)
$$

> the restriction of an universal quantification is the same as conditional statement
>
> the restriction of an existential quantification is the same as conjunction

### Precedence

annotation like
$$
\exist \\ \forall
$$
have a higher procedure than other annotations

### Binding Variables

$$
\forall x (x+y=z)
$$

x: bound

y,x : free

**scope**: the expression that the variable is applied 
$$
the \  scope \  \  of \  \forall  \  is  \ (x+y=z)
$$

### Logical Equivalences

Statements involving predicates and quantififiers are *logically equivalent*

if and only if they **have the same truth value** no matter which

predicates are substituted into these statements and which **domain of**

**discourse is used** for the variables in these propositional functions. We

use the notation *S* *≡* *T* to indicate that two statements *S* and *T*

involving predicates and quantififiers are logically equivalent.
$$
\forall x(P(x)\wedge Q(x)) ≡ \forall x(P(x)) \wedge \forall Q(x)
$$

$$
De \ Morgan's  \ Law\\
¬∀x P(x) ≡ ∃x ¬P(x) \\
¬∃x P(x) ≡ ∀x ¬P(x)
$$

### All logical laws

![QQ截图20220920102431](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220920102431.png)

![QQ截图20220920102535](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220920102535.png)

![QQ截图20220920102549](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220920102549.png)

![QQ截图20220920102556](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220920102556.png)

### Nested Quantifiers

$$
\forall x \exist y (x+y=0)
$$

both x and y are bound

scope: (x+y=0)

**When quantifiers are of the same quantity (all universal or all existential), the order does not matter.**

**But when they are mixed, the order becomes crucial.**  

### Negating Nested Quantifiers  

**example**
$$
\neg \forall x \exist y (xy = 1) \\
\exist x \neg \exist y (xy=1)  \\
\exist x \forall y (xy \ != 1)
$$

### Homework

prove that 
$$
\forall x (P(x) \wedge Q(x)) \ ≡ \ \forall x P(x) \wedge \forall x Q(x)
$$

> the proof should use twice that is from left to right and from right to left. 

> the proof is just using natural language but not using logical annotation

