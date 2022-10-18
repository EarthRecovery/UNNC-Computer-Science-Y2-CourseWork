# Week02 Inference rules

>  section 1.6

### Argument

​        An **argument** in propositional logic is a sequence of propositions. All but the final proposition in the argument are called **premises** and the final proposition is called the **conclusion**. An argument is valid if the truth of all its premises implies that the conclusion is true.  

>  argument form  is true + premises are all true ==> conclusion is true

## Inference Rules for Propositional Logic  

### Modus Ponens  

![QQ截图20220927094539](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094539.png)

### Modus Tollens  

![QQ截图20220927094708](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094708.png)

### Hypothetical syllogism  

![QQ截图20220927094742](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094742.png)

### Disjunctive syllogism  

![QQ截图20220927094806](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094806.png)

### Addition  

![QQ截图20220927094831](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094831.png)

### Simplification  

![QQ截图20220927094857](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094857.png)

### Conjunction  

![QQ截图20220927094917](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094917.png)

### Resolution  

![QQ截图20220927094941](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927094941.png)

**exercise**

![QQ截图20220927100354](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927100354.png)
$$
\neg(\neg q \vee \neg p)\wedge q \\
= (q \wedge p) \wedge q \\
p \ is \ true\\
\\
\neg(\neg q \wedge \neg p) \ is \ true \\
\\

that \ is  \ to \ prove \ p \rightarrow r \ is \ true \\
r \ is \ true \\
Q.E.D
$$
![微信图片_20220927101546](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\微信图片_20220927101546.jpg)

## Rules of Inference for Quantified Statements  

### Universal instantiation  

![QQ截图20220927101917](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927101917.png)

### Universal Generalization  

![QQ截图20220927101958](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927101958.png)

### Existential Instantiation  

![QQ截图20220927102044](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927102044.png)

### Existential Generalization  

![QQ截图20220927102126](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927102126.png)

### exercise1

![QQ截图20220927102205](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927102205.png)

D(x) one is in discrete class

C(x) x has taken a course in CS
$$
\forall x (D(x) \rightarrow C(x)) \\
D(Marla) \ is \ true \\ 
C(Marla) \ is \ true
$$

### exercise2

![QQ截图20220927104250](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\QQ截图20220927104250.png)

C(x) x is in the class

B(x) x has read the book

P(x) x has pass the exam

![微信图片_20220927104223](C:\Users\earth_recovery\Desktop\Learning\UNNC Y2 First Semester\Mathematics for Computer Scientists (COMP1046 UNNC)\assests\微信图片_20220927104223.jpg)

### exercise3

