##### Exercise 3.2.1
- Axiom 3.2
Let $P(x)$ be a property pertaining to $x$ such that $P(x)$ is always false. We know that the set $\{x : P(x)\}$ exists and from how we defined $P(x)$ we also know that $x \notin \{x : P(x)\}$ which is the definition of $\emptyset$, thus we axiom 3.8 implies axiom 3.2.
- Axiom 3.3
Let $P(x)$ be a property pertaining to $x$ such that $P(x)$ is true iff $x = a$ or $x = b$. From axiom 3.8 we know that $a \in \{x : P(x)\}$ and $b \in \{x : P(x)\}$ and no other object is an element of that set, which is the definition of $\{a,b\}$ and since we know that pair sets imply singleton sets we can see that axiom 3.8 implies axiom 3.3
- Axiom 3.4
Let's say that $A$ and $B$ are sets. We can define a property $P(x)$ such that $P(x) = (x\in A \text{ or } x\in B)$. Thus we know that the set $\{x: P(x)\}$ exists and this set is equal to set $A \cup B$ from definition 3.1.4, thus axiom 3.8 implies axiom 3.4.
- Axiom 3.5
We already know that axiom 3.6 implies axiom 3.5 thus we only need to show that axiom 3.8 implies axiom 3.6
- Axiom 3.6
Let $P(y)$ be a property pertaining to $y$ such that $P(y)$ is true iff $Q(x, y) \text{ is true for some } x\in A$, we already know that the set $\{y : P(y)\}$ exists, thus $\{y : Q(x,y) \text{ for some }x \in A\}$ also exists. 
We also know that $z \in \{y: P(y)\} \iff P(z)$ from axiom 3.8 thus $z \in \{y: Q(x, y) \text{ is true for some x} \in A\} \iff Q(x,z) \text{ is true for some x} \in A$ showing that axiom 3.8 implies axiom 3.6
##### Exercise 3.2.2
Let's say that $A$ is a set. We know that $\{A\}$ is a non-empty set from axiom 3.3. The set $\{A\}$ has only one element and that element is a set thus by axiom 3.9 A must be disjoint from $\{A\}$, showing that $A$ cannot contain $A$.
Let's say that $B$ is also a set. We know that $\{A, B\}$ is a non-empty set from axiom 3.3. From axiom 3.9 the set $\{A,B\}$ must have an element that is either not a set or is disjoint from itself. We already know that $A$ and $B$ cannot contain themselves thus for $A$ to be disjoint it suffices that $A \notin B$ and for B to be disjoint it suffices that $B \notin A$. Because of axiom we know that either A or B or both of them needs to be disjoint from the set $\{A,B\}$ thus either $A\notin B$ or $B \notin A$ or both. 
##### Exercise 3.2.3
Let's assume that the universal set $\Omega$ exists. For axiom 3.8 to be true we need to show that for a property $P(x)$ pertaining to $x$ there exists a set $\{x : P(x) \text{ is true}\}$ such that $y \in \{x : P(x) \text{ is true}\} \iff P(y) \text{ is true}$. We already know that every element $x$ where $P(x) \text{ is true}$ is already an element of $\Omega$ and using axiom 3.5 we can see that the set $\{x\in \Omega : P(x) \text{ is true }\}$ exists and $y\in \{x\in \Omega : P(x) \text{ is true }\} \iff \{y \in \Omega \text{ and } P(y) \text{ is true}\}$ thus the universal set $\Omega$ implies axiom 3.8.
Let's assume axiom 3.8. We need to show that the universal set $\Omega$ exists. Let's say that property $P(x)$ pertaining to $x$ is true for all objects. By axiom 3.8 we can say that the set $\{x:P(x)\text{ is true }\}$ exists which is the definition of the universal set. We have shown that universal set $\Omega$ exists iff axiom 3.8 is true.