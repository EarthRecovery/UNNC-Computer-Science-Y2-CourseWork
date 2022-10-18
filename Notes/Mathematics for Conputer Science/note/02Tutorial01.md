# Tutorial01

### Q1

**use a truth table to prove its tautology**
$$
( 𝑝 → (𝑞 ∨ 𝑟) ↔ (𝑝 ∧ ¬𝑞) → 𝑟)
$$

$$
 (𝑝 → (𝑞 → 𝑟)) ↔ ((𝑝 ∧ 𝑞) → 𝑟)
$$

try to use the truth table, it's easy anyway.



### Q2

1. **Show that (𝑝 → 𝑟) ∨ (𝑞 → 𝑟)and (𝑝 ∧ 𝑞) → 𝑟 are logically equivalent**

$$
(p \wedge q) \rightarrow r \\
=\neg (p \wedge q) \vee r  \ || \ rule(20)\\
=(\neg p \vee \neg q) \vee r \ || \ De \ Morgan's  \ laws\\
=(\neg p \vee r) \vee (\neg q \vee r) \\
=(p \rightarrow r) \vee (q \rightarrow r)
$$

2. **Show that ¬𝑝 → (𝑞 → 𝑟) and 𝑞 → (𝑝 ∨ 𝑟) are logically equivalent**

$$
¬𝑝 → (𝑞 → 𝑟) \\
=p \vee (\neg q \vee r) \ || \ rule(20)\\
=\neg q \vee (p \vee r) \ || \ commutative \ laws\\
=𝑞 → (𝑝 ∨ 𝑟) \ || \ rule(20)
$$

3. **Show that (p→ q) → r and p→ (q → r) are not  equivalent**  
$$
(p→ q) → r  \\
   =\neg (\neg p \vee q) \vee r \  || \ rule(20)\\
   =(p \wedge  \neg q) \vee r \  || \ De \ Morgan's \ law \\
$$

   

$$
p→ (q → r) \\
=\neg p \vee (\neg q \vee r) \  || \ rule(20) \\
=(\neg p \vee \neg q) \vee r \  || \ commutative \ law
$$

in this case: 
$$
(p \wedge q) \vee r \ \ != (\neg p \vee \neg q) \vee r
$$

### Q3

**Let 𝑃 𝑥 , 𝑄 𝑥 , and 𝑅 𝑥 be the statements “𝑥 is a professor,”  “𝑥 is ignorant,” and “𝑥 is vain,” respectively. Express each of these statements using quantifiers; logical connectives; and 𝑃 𝑥 , 𝑄 𝑥 , and 𝑅 𝑥 , where the domain consists of all people.**
a) No professors are ignorant.
$$
\forall x \neg (P(x) \wedge Q(x))
$$
b) All ignorant people are vain.
$$
\forall x Q(x) \rightarrow R(x)
$$
c) No professors are vain.
$$
\neg \exists x P(x) \wedge R(x)
$$
d) Does (c) follow from (a) and (b)?  
$$
no, for \ \ not  \ \ all \ \ vain \ \ people \ \ are \ \ ignorant
$$

### Q4

**Use quantifiers to express the statement that “There is a woman who has taken a flight on every airline in the world.”**  

P(x) a person is a women

Q(x) a person take a flight on every airline in the world
$$
\exists x P(x) \wedge Q(x)
$$
**Use quantifiers to express the statement that “There does not exist a woman who has taken a flight on every airline in the world.”**  
$$
\neg \exists x P(x) \wedge Q(x)
$$

### Q5

**Suppose that the domain of 𝑄 𝑥, 𝑦, 𝑧 consists of triples 𝑥, 𝑦, 𝑧 , where 𝑥 = 0, 1, 𝑜𝑟 2, 𝑦 = 0 𝑜𝑟 1 , 𝑎𝑛𝑑 𝑧 = 0 𝑜𝑟 1 . Write out these propositions using disjunctions and conjunctions.**
a) ∀y Q(0, y, 0)
$$
Q(0,0,0) \wedge Q(0,1,0)
$$
b) ∃𝑥 𝑄 (𝑥, 1,1)
$$
Q(0,1,1) \vee Q(1,1,1)\vee Q(2,1,1)
$$
c) ∃z¬ 𝑄(0,0, 𝑧)
$$
?
$$
d) ∃𝑥¬ 𝑄(𝑥, 0,1)  
$$
?
$$

### Q6

**Use rules of inference to show that if ∀𝑥 (𝑃 (𝑥) → (𝑄 (x) ∧ 𝑆 (𝑥))) and ∀𝑥(𝑃 (𝑥) ∧ 𝑅 (𝑥) ) are true, then ∀𝑥(𝑅 (𝑥) ∧ 𝑆 (𝑥) ) is true.**  
$$

$$
