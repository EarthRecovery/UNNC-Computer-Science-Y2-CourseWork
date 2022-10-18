# Week02 proof

### Reading

- Secton1.8
- section 5.1
- section 5.2

### direct proof and indirect proof

If a proof leads from the premises of a theorem to the conclusion, then
it is a direct proof, otherwise, it is an indirect proof.  

A **direct proof** shows that a conditional statement p ! q is true by
showing that  

**if p is true, then q must also be true**  

#### exercise

‘If n is an odd integer, then n2 is odd’.  

**proof:**

Suppose n is an odd integer. Then there exists an integer k such that n = 2k + 1. n2 = (2k + 1)^2 = 4k^2 + 4k + 1 = 2(2k2 + 2k) + 1. Since 2(k^2 + 2k) is an integer, n2 is odd.

### Proof by Contraposition  (indirect proof)

$$
 if \ p \rightarrow q \ then \\
 \neg q \rightarrow \neg p
$$

#### exercise

Prove that **if n is an integer and 3n + 2 is odd, then n is odd.**  

**proof:**

p : 3n+2 is odd;

q : n is odd

it is the same meaning that: 

**if n is even then proof 3n+2 is even**

let n=2k, 3n+2 = 6k+2 = 2(3k+1)

because 3k+1 is integer

6k+2 is even

Q.E.D.

### Proof by Contradiction  (indirect proof)

Because the statement
$$
r \wedge \neg r
$$
is a contradiction whenever r is a proposition, we can prove that p is true if we can show that
$$
\neg p \rightarrow (r \wedge \neg r)
$$
 is true for some proposition r.  

#### Exercise  

Prove that 
$$
\sqrt{2} \ is \ irrational
$$
![QQ截图20220929102650](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929102650.png)



### Proof of Equivalence  

To prove a theorem that is a biconditional statement or a bi-implication,
that is, a statement of the form 
$$
p \leftrightarrow q
$$
 we show that
$$
p \rightarrow q
$$
and 
$$
q \rightarrow p
$$
are both true.  

**so:** 

![QQ截图20220929103814](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929103814.png)![QQ截图20220929103744](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929103744.png)

### Counterexamples  

<img src="C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929103941.png" alt="QQ截图20220929103941" style="zoom:150%;" />

#### exercise

Show that the statement **‘Every positive integer is the sum of the**
**squares of two integers’** is false  

**proof:**

**3 is not include**

### Proof by Cases  

![QQ截图20220929104445](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929104445.png)

#### exercise

![QQ截图20220929104359](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220929104359.png)

### Mathematical Induction  (数学归纳法)

**Basis Step**: We show that the statement holds for the positive
integer 1 (i.e. P(1) is true).
**Inductive Step** We show that if the statement holds for a positive
integer then it must also hold for the next larger integer (i.e. for all
positive integers k, if P(k) is true, then P(k + 1) is true).  ![QQ截图20221011090701](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20221011090701.png)

### Strong Induction  

![QQ截图20221011092822](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20221011092822.png)
