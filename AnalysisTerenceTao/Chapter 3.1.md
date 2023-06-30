##### Exercise 3.1.1
Let's say there are three sets A, B and C.
- Equality in sets is reflexive.
We know that $x \in A$ iff $x \in A$ because they are the same statement, thus $A = A$ from definition 3.1.4. $\square$

- Equality in sets is symmetric
We need to prove that if $A = B$ then $B = A$.
We need to show that $x \in A$ iff $x \in B$ implies $x \in B$ iff $x \in A$. We know that iff is symmetric thus $B = A$ from definition 3.1.4. $\square$

- Equality in sets is transitive
We need to show that if $A = B$ and $B = C$, then $A = C$.
Using definition 3.1.4 we can see that $x \in A \iff x \in B$ and $x \in B \iff x \in C$, thus $x \in A \iff x \in C$ which implies $A = C$ by definition 3.1.4 $\square$ 
##### Exercise 3.1.2
We know that from Axiom 3.2 and Axiom 3.3 that all of these sets are objects. From definition 3.1.4 we know that to prove they are different from each other it is sufficent to show that an element of one set doesn't belong to another set.
$\emptyset \notin \emptyset$, $\emptyset \in \{\emptyset\}$, $\emptyset \in \{\emptyset, \{\emptyset\}\}$ and $\{\emptyset\} \notin \emptyset$, $\{\emptyset\} \in \{\{\emptyset\}\}$ thus the set $\emptyset$ is different from all the other sets.
$\{\emptyset\} \notin \{\emptyset\}$, $\{\emptyset\} \in \{\{\emptyset\}\}$, $\{\emptyset\} \in \{\emptyset, \{\emptyset\}\}$ thus the set $\{\emptyset\}$ is different from all the other sets.
$\emptyset \notin \{\{\emptyset\}\}$, $\emptyset \in \{\emptyset, \{\emptyset\}\}$ thus they are different from each other and this is sufficent enough to show that all of the sets are distinct. $\square$
##### Exercise 3.1.3
- Union operation is commutitive
Let's say that $x \in A\cup B$ there are two cases, $x \in A$ or $x \in B$.
From the Axiom 3.4 we know that $x \in A$ implies $x \in B \cup A$ and $x \in B$ implies $x \in B \cup A$ thus we have shown that $x \in A \cup B$ implies $x \in B \cup A$.  Using a similar argument we can show that the opposite is also true, thus by definition 3.1.4 $A \cup B = B \cup A$. $\square$

- $A \cup A = A \cup \emptyset = \emptyset \cup A = A$ 
First we'll look at $A \cup A$. From the Axiom 3.4 we know that there are two cases $x \in A$ and $x \in A$ but as we can see they are the same case so we don't need to look at them seperately. From definition 3.1.4 we need to show that $x \in A$ iff $x \in A$ to prove $A \cup A = A$ but as we can clearly see they are the same statement thus finishing the proof.
Because we know that union operation is commutitive we only need to show that $A \cup \emptyset = A$. Similarly we will look at this in two cases. $x \in A$ and $x \in \emptyset$ but we already know that there aren't any element in the $\emptyset$ from Axiom 3.2 thus we only need to look at the case $x \in A$ and using the same logic as before we can show that $A \cup \emptyset = A$. $\square$
##### Exercise 3.1.4
- If $A \subseteq B$ and $B \subseteq A$, then $A = B$ 
We know from definition 3.1.15 that $A \subseteq B$ implies that for any object $x$, $x \in A \implies x \in B$ and $A \subseteq B$ implies that for any object $x$, $x \in A \implies x \in B$. If we combine these two statements we get for any object $x$, $x \in A \iff x \in B$ and this is the definition of $A = B$ thus we have finished the proof. $\square$ 

- If $A \subset B$ and $B \subset C$ then $A \subset C$ 
We already know that this holds for improper subsets so we only need to show that $A \neq C$. From definition 3.1.15 we know that $A \subset B \implies A \neq B$. By definition 3.1.4 For $A \neq B$ to be true $\exists x, x \in A , x \notin B$ or $\exists x,x \notin A,x \in B$. We know that there cannot be an $x$ such that $x \in A$ and $x \notin B$ because $A \subset B$ thus there must exist an $x$ that satisfies $x\notin A$ and $x \in B$. Because $B \subset C$ that $x$ must also be an element of $C$ thus $\exists x, x \notin A, x\in B, x\in C$ proving that $A \neq C$. $\square$ 
##### Exercise 3.1.5
- $A \subseteq B \iff$ (for any object $x, x \in A \implies x \in B$)       
- $A \cup B = B$ 
From definition 3.1.4 and Axiom 3.4 we know that  $\forall x, (x \in A \text{ or } x\in B) \iff x \in B$ thus $\forall x, x \in A \implies x\in B$ and  $\forall x, x \in B \implies x\in B$. The second case is vacuosly true and the first case is the definition of $A \subseteq B$.
- $A \cap B$ = A
Let's say that there exists an $x$ such that $x \in A$. We know that $A = A\cap B$ thus $x \in A \cap B$ from definition 3.1.4. By definition 3.1.23 we can conclude that $x \in A \implies x \in A$ and $x \in A \implies x \in B$. The first statement is vacuosly true and the second statement is the definition of $A \subseteq B$.  $\square$ 
##### Exercise 3.1.6
$A,B,C \subseteq X$ 
- (a) $A \cup \emptyset = A$ and $A \cap \emptyset = \emptyset$ 
From exercise 3.1.3 we know that $A \cup \emptyset = A$ so we only need to prove the second statement. From definition 3.1.23 we know that for an $x$ to be an element of $A \cap \emptyset$ it needs to be an element of $A$ and $\emptyset$ but from axiom 3.2 we know that no object is an element of the empty set thus no object is an element of $A \cap \emptyset$. By definition 3.1.4 it is equal to the empty set. $\square$ 
- (b) $A \cup X = X$ and $A \cap X = A$ 
First we'll look at $A \cup X = X$. Let's assume $x \in A \cup X$. We know that from axiom 3.4 that $x \in X$ or $x \in A$ so we'll look at both cases. We already know that $x \in X \implies x\in X$ and from definition 3.1.15 we know that $x \in A \implies x \in X$ thus $x \in A\cup X \implies x \in X$. Now let's assume $x \in X$ and show that $x \in A \cup X$. From axiom 3.4 we know that it is sufficent to show that either $x \in A$ or $x \in X$ for $x \in A\cup X$ to be true and we already know that $x\in X$ thus $x\in X \implies x \in A \cup X$ thus $x\in X \iff x \in A \cup X$ and by definition 3.1.4 we have shown that  these two sets are equal.
By definition 3.1.23 we can rewrite $x\in A\cap X$ as $x \in A \text{ and } x \in X$. Using definition 3.1.15 we know that $x \in A \implies x\in X$ thus the statement can be concisely written as $x\in A and by definition 3.1.4 this is sufficent to show that $A\cap X = A$. $\square$ 
- (c) $A \cap A = A$ and $A \cup A = A$ 
In exercise 3.1.3 we have already shown that $A \cup A = A$. Using definition 3.1.4 and definition 3.1.23 we can rewrite $A \cap A = A$ as $(x \in A \text{ and } x\in A) \iff x \in A$. As you can see it is trivial to show that that statement is true. $\square$
- (d) $A \cup B = B \cup A$ and $A \cap B = B \cap A$
in exercise 3.1.3 we have already shown that union operation is commutative. Using definition 3.1.4 we can rewrite $A \cap B = B \cap A$ as $x \in A \cap B \iff x \in B \cap A$ and by definition 3.1.23 this is equivalent to $(x \in A \text{ and } x\in B) \iff (x \in B \text{ and } x \in A)$. We already know that the logical and operation is commutative thus intersection operation is also commutative. $\square$
- (e) $A \cup (B \cup C) = (A \cup B) \cup C$ and $A \cap (B \cap C) = (A \cap B) \cap C$ 
In lemma 3.1.13 we have already shown that union operation is commutative.
By definition 3.1.4 we need to show that every element of $A \cap (B \cap C)$  is also an element of $(A \cap B) \cap C$. Let's say that $x$ is an element of $A \cap (B \cap C)$. By definition 3.1.23 this means that $x \in A$ and $x \in B \cap C$ and from definition 3.1.23 we know that $x \in B$ and $x \in C$.
We know that $x\in A$ and $x \in B$ thus by definition 3.1.23 $x \in A \cap B$. We also know that $x \in C$ so using definition 3.1.23 we can show that $x \in (A\cap B)\cap C$. A similar argument shows that every element in $(A \cap B) \cap C$ is also an element of $A \cap (B \cap C)$ and so $A \cap (B \cap C) = (A \cap B) \cap C$ $\square$ 
- (f) $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$ and $A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$
We'll prove the first statement first. Let's say that $x \in A \cap (B\cup C)$. By definition 3.1.23 we know that $x \in A$ and $x \in B \cup C$. By axiom 3.4 we can look at this in two cases. Either $(x\in A \text{ and } x\in B)$ or $(x \in A \text{ and } x\in C)$ and by axiom 3.4 and definition 3.1.23 this is equivalent to $(A \cap B) \cup (A \cup C)$. We can show that the other statement is true using a similar argument thus we finish the proof. $\square$ 
- (g) $A\cup(X\setminus A) = X$ and $A\cap (X \setminus A) = \emptyset$
Let's say that $x\in A\cup(X\setminus A)$, we can rewrite this as $x\in A \text{ or } (x \in X \text{ and } x \notin A)$ using definition 3.1.4 and definition 3.1.27. By definition 3.1.15 we already know that $x\in A \implies x\in X$ thus we can rewrite the set as ($x\in A \text{ and } x\in X) \text{ or } (x \in X \text{ and } x \notin A)$. We already know that an object is either an element of a set or not element of a set thus $x$ must be an element of set $X$.
Let's say that $x\in A\cup(X\setminus A)$, we can rewrite this as $x\in A \text{ and } (x \in X \text{ and } x \notin A)$ using definition 3.1.4 and definition 3.1.27. But we know that an object can't be an element of a set and not an element of a set thus there can't exists an $x$ that satisfies these conditions, thus $\forall x, x \notin  A\cap(X\setminus A)$. From lemma 3.1.6 we can see that this set is equivalent to $\emptyset$ thus completing the proof $\square$ 
- (h) $X\setminus(A\cup B) = (X\setminus A) \cap (X \setminus B)$ and $X\setminus(A\cap B) = (X\setminus A) \cup (X \setminus B)$
By definition 3.1.27 and definition 3.1.23 we can rewrite $x\in (X\setminus A)\cap (X\setminus B)$ as $(x\in X \text{ and } x\notin A) \text{ and } (x\in X \text{ and } x\in B)$ which can be concisely written as $x \in X \text{ and } x \notin A \text{ and } x\notin B$.
We can rewrite $x \in X\setminus (A \cup B)$ as $x \in X \text{ and } x\notin (A \cup B)$ using definition 3.1.27. We know from axiom 3.4 that $x \notin (A \cup B) \iff (x \notin A \text{ and } x \notin B)$, thus we have shown that $x \in X \text{ and } x \notin A \text{ and } x\notin B$ proving that two statements are equivalent and from definition 3.1.4 equal. We can prove the second statement using a similarargument. $\square$ 
##### Exercise 3.1.7
- $A \cap B \subseteq A$ and $A \cap B \subseteq B$
Since we already know that intersection operation is commutitive from exercise 3.1.6d only showing one of them is true will suffice. By definition 3.1.15 we need to prove that $x\in A\cap B \implies x\in A$ and using definition 3.1.23 we can rewrite this as $(x\in A \text{ and } x\in B) \implies x\in A$ which is true.
- $C \subseteq A \text{ and } C \subseteq B \iff C \subseteq A \cap B$ 
By definition 3.1.15 and definition 3.1.23 we can rewrite $C \subseteq A \cap B$ as $x\in C \implies (x\in A \text{ and } x\in B)$ which we can write as seperate statements $x\in C \implies x\in A$ and $x \in C \implies x \in B$. Using definition 3.1.15 these two statements can be rewritten as $C \subseteq A$ and $C \subseteq B$ thus finishing the proof.
- $A \subseteq A \cup B$ and $B \subseteq A\cup B$
Since we know that pairwise union is commutitive only proving one of the statements is sufficent. By definition 3.1.15 we need to show that $x \in A \implies x \in A \cup B$. From axiom we already know that this is the case thus completing the proof.
- $(A \subseteq C \text{ and } B\subseteq C) \iff A\cup B\subseteq C$.
Let's assume $A \subseteq C$ and $B \subseteq C$. By definition 3.1.15 we can rewrite $(A \subseteq C \text{ and }B \subseteq C)$ as  $x \in A \implies x\in C$ and $x \in B \implies x \in C$, and we can combine those two statements as $(x\in A \text{ or } x\in B) \implies x\in C$. From axiom 3.4 we know that $x\in A \text{ or } x\in B \iff x\in A\cup B$, thus $x\in A\cup B \implies x\in C$ which equivalent to $A\cup B\subseteq C$ by definition 3.1.15.
##### Exercise 3.1.8
$A \cap (A \cup B) = A$ and $A \cup (A\cap B) = A$
We'll start with $A \cap (A \cup B)$. From definition 3.1.23 it is trivial to see that $x \in A \cap (A \cup B) \implies x \in A$ so we only need to show the other way around to see that they are equal by definition 3.1.4. From axiom 3.4 we can see that $x\in A \implies x\in (A \cup B)$ and we already know that $x \in A \implies x \in A$, thus by definition 3.1.23 we know that $x \in A \implies x \in A \cap (A \cup B)$ meaning that $A \cap (A \cup B) = A$. We can make a similar argument for the other statement completing the proof. $\square$
##### Exercise 3.1.9
$(A \cup B = X \text{ and } A \cap B = \emptyset) \implies (A = X\setminus B \text{ and } B = X\setminus A)$ 
Let's assume $x \in X$. $A\cap B = X$ implies that $x \in A$ or $x \in B$ or both, but since we know by axiom 3.2, definition 3.1.4 and definition 3.1.23 $A \cap B = \emptyset$ implies that there exists no object that is both an element $A$ and an element $B$, $x$ must either be an element $A$ or an element of $B$. Now we have everything we need to prove the right side of the original statement.
Since we know that intersection is commutitive, the same argument can be applied with $A$ and $B$ swapped, thus only showing $A  = X\setminus B$ is true is sufficent. We know that every element in $X$ is either an element of $A$ or an element $B$ and when we remove the elements that are in $B$ using difference operation all that we are left with is the elements that are in $A$. We also know that all the objects that are an element of $A$ is also an element of $X$ thus by defintition 3.1.4 we know that $A = X \setminus B$. $\square$ 
##### Exercise 3.1.10
Sets $A \setminus B$, $A \cap B$, and $B \setminus A$ are disjoint and their union is $A \cup B$
Using axiom 3.4 we can split $x\in A\cup B$ into three distinct cases.
Either $x$ is an element of $A$ or $x$ is an element of $B$ or $x$ is an element of both. Using definition 3.1.23 and definition 3.1.27 we can show that these cases are $A\setminus B$,$B\setminus A$ and $A\cap B$ respectively. We haven't yet shown that they are mutually exclusive but we know that their union is $A\cup B$. Let's say that for the sake of contradiction that there exists an $x$ such that $x \in A\setminus B, x\in B\setminus A$. From definition 3.1.27 that would mean that $x \in A \text{ and } x \notin B$ and $x \notin A \text{ and } x\in B$ thus a contradiction. Similar arguments can be made for all of the other cases thus completing the proof. $\square$ 
##### Exercise 3.1.11
Axiom of replacement implies axiom of specification
First we'll assume axiom of replacement is true, thus we know that if there exists a set $A$ and a property $P(x,y)$ pertaining to $x$ and $y$ such that foreach $x$ there exists at most one y that makes $P(x, y)$ true, then there exists a set such that $\{y : P(x, y) \text{ is true for some } x \in A\}$. We need to show that for a set $B$ and property $Q(x)$ pertaining to $x$ there exists a set $\{x \in B : Q(x)\}$. If we let  $P'$ be a property such that $P'(x, x)$ is true $\iff$ $Q(x)$ and $P'$ is false otherwise, we can see that $\{y : P'(x,y) \text{ is true for some }x\in B\} = \{x\in B : Q(x)\}$ thus proving that the set exists.