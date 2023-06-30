##### Axiom 2.4
$\newcommand{\pp}{\verb!++!}$If $n\pp = m\pp$, then $n = m$
##### Definition of Addition
$0 + m := m$
$(n\pp) + m := (n+m)\pp$
##### Lemma 2.2.1a
The sum of two natural numbers is again a natural number.
We need to show that $n + m$ is a natural number where $n$ and $m$ are a natural numbers. We'll induct on n while keeping m fixed. 
For the base case we already know that $0 + m = m$ which is a natural number. We'll inductively assume that $n + m$ is a natural number and we need to show that $(n\pp) + m$ is also natural number. From the definition of addition $(n\pp) + m = (n + m)\pp$. We know that from the inductive hypothesis that $n + m$ is a natural number and from Axiom 2.2 that $(n + m)\pp$ is also a natural number thus closing the induction $\square$
##### Lemma 2.2.2
$n + 0 = n$
##### Lemma 2.2.3
$n + (m\pp) = (n+m)\pp$
##### Proposition 2.2.4
$n + m = m + n$
##### Proposition 2.2.5
Prove that $(a + b) + c = a + (b + c)$
We'll use induction on b while keeping a and c fixed. 
First we need to prove the base case $(a + 0) + c = a + (0 + c)$
By the definition of addition, $0 + c = c$ thus the right side is equal to $a +c$. 
By Lemma 2.2.2, $a + 0 = a$ so the left side is also equal to $a + c$ thus proving the base case.
Now we'll assume inductively that $(a + b) + c = a + (b + c)$ and prove $(a + (b\pp)) + c = a + ((b\pp) + c)$. From Lemma 2.2.3 the left-hand side equals $((a + b)\pp) + c$ and from the definition of addition $((a + b) + c)\pp$. 
Similarly, the right-hand side equals $a + ((b + c)\pp)$ from the definition of addition and $(a + (b + c))\pp$ from Lemma 2.2.3. By the inductive hypothesis right-hand side is equal to  $((a + b) + c)\pp$.
Now that we have shown that both sides are equal, this closes the induction. $\square$
##### Proposition 2.2.6
If $a + b = a + c$, then $b = c$
##### Definition 2.2.7
A natural number is positive iff it is not equal to 0
##### Proposition 2.2.8
If $a$ is a positive number and $b$ is a natural number, then $a + b$ is positive.
##### Corrolary 2.2.9
If $a$ and $b$ are natural numbers such that $a + b = 0$, then $a = 0$ and $b = 0$
##### Lemma 2.2.10
Let $a$ be a positive number. There exists exactly one natural number such that $b\pp = a$.
First we know that there can at most one such natural number $b$ because of Axiom 2.4 so we only need to show that b exists.
We'll use induction on $a$. The base case is $a = 1$. We know that $1 = 0\pp$ from the definition of $1$ so $b = 0$ when $a = 1$ thus we have shown the base case.
Now we'll inductively assume there exists a natural number $b$ such that $b\pp = a$ and we'll need to show that there exists a natural number $c$ such that $c\pp = a\pp$. From the Axiom 2.4 we know that $c = a$ and from the definition of $a$ we know that c is a positive number thus a natural number closing the induction $\square$ 
##### Definition of Ordering of the natural number
$n \ge m$ or $m \le n$ iff $n = m + a$ for some natural number $a$
$n \gt m$ or $m \lt n$ iff $n \ge m$ and $n \ne m$.
##### Proposition 2.2.12
(a ) $a \ge a$. Order is reflexive 
From the definition of addition and Proposition 2.2.4 we know that $a = a + 0$ which proves that $a \ge a$ by the definition of ordering. 

(b) If $a \ge b$ and $b \ge c$, then $a \ge c$. Order is transitive
We know that $a = b + x$ and $b = c + y$ where $x$ and $y$ are some natural number thus $a = c + y + x$ and $a = c + (y + x)$ from Proposition 2.2.5. From Lemma 2.2.1a we know that $y + x$ is also a natural number and this is enough to show that $a \ge c$.

(c) If $a \ge b$ and $b \ge a$, then $a = b$. Order is anti-symmetric
From the definition of ordering we know that $a = b + x$ and $b = a +y$ where $x$ and $y$ are natural numbers thus $a = a + (y + x)$. 
From the definition of addition this is equal to $a + 0 = a + (y + x)$ and using the Proposition 2.2.6 we can show that $0 = y + x$
$y = 0$ and $x = 0$ from Corrolary 2.2.9 and using this we can show that $a = b + 0$. By Lemma 2.2.2 we can show that $a = b$ $\square$

(d) $a \ge b$ iff $a + c \ge b + c$. Addition preserves order
We know that from that from the definition of ordering that $a + c \ge b + c$ iff $a + c = b + c + x$ where $x$ is a natural number. 
From Proposition 2.2.6 we can show that $a + c \ge b + c$ iff $a = b + x$ which is equivalent to $a \ge b$ from the definition of ordering thus completing the proof. $\square$ 

(e) $a \lt b$ iff $a\pp \le b$.
Suppose $a \le b$, thus $a = b + c$ and $a \ne b$. We know that $c$ is positive from (f) thus $c = x\pp$ from Axiom 2.2 where x is a natural number. 
$b = a + (c\pp)$ 
$b = (a + c)\pp$ from the Lemma 2.2.3
$b = (a\pp) + c$ from the definition of addition
$b \ge a\pp$ or $a\pp \le b$ thus completing the proof. $\square$

(f) $a \lt b$ iff $b = a + d$ for some positive number $d$.
We know that from the definition of ordering that $a \lt b$ iff $b = a + c$ and $b \ne a$ where c is a natural number. Let's assume for the sake of contradiction that $c = 0$. We know that from Lemma 2.2.2 that $b = a + 0$ implies $b = a$ thus contradicting $b \ne a$. Now we know that $a < b$ iff $b = a + c$ where c is not 0 and a natural number, we also don't need to mention that $b \ne a$ when writing the iff statement because we have shown that when c is a positive number, $b = a + c$ implies that $b \ne a$. The statement we arrived is the same as the one we want thus finishing the proof. $\square$ 
##### Proposition 2.2.13
(a) $0 \le b$ for all b
We know that $0 + b = b$ from the definition of addition, this statement is equivalent to $0 \le b$ by the definition of ordering. $\square$ 

(b) If $a > b$ then $a\pp > b$ 
We'll assume $a > b$. From Proposition 2.2.12f we know that $a = b + d$ where d is a positive number. 
$a\pp = (b + d)\pp$
$a\pp = b + (d\pp)$ from Lemma 2.2.3 and because we know that $d\pp$ is not zero from Axiom 2.3 we can conclude that $d\pp$ is a positive number. Now we can show that $a\pp > b$ using Proposition 2.2.12f thus finishing the proof. $\square$ 

(c) If $a = b$ then $a\pp > b$ 
We need to show that $a\pp = b + c$ for some positive number c because of Proposition 2.2.12f. We know that $a = b + 0$ by Lemma 2.2.2 and we can show that $a\pp = (b + 0)\pp$ is equivalent to $a\pp = b + (0\pp)$ using Lemma 2.2.3. We know that $0\pp$ is not 0 from Axiom 2.3 thus $0\pp$ is a positive number and we have shown that $a\pp > b$. $\square$
##### Proposition 2.2.14
We know that if $P(m')$ is true for all natural numbers $m_0 \le m' \le m$, then $P(m)$ is also true. We need prove that we can conclude that $P(m)$ is true for all natural numbers $m \ge m_0$.
We'll show that $P(m)$ is true for all m using induction. We know that the base case $P(m_0)$ has to be true because there is no natural number that satisfies the condition $m_0 < m_0$. Now we will inductively assume that $P(m)$ is true and prove that $P(m\pp)$ is also true. If $P(m)$ is true, then $P(x)$ is true for all natural numbers $m_0 \le x < m$ . We know from Proposition 2.2.13c that $m < m\pp$ thus we can conclude that $P(x)$ is true for all natural numbers $m_0 \le x < m\pp$ and this is enough to prove that $P(m\pp)$ is also true, closing the induction. ??
##### Exercise 2.2.6
We'll use induct on $n$ to prove that $P(m)$ is true for all natural numbers $m \le n$.
The base case $n = 0$ is trivial to see because we know only natural number m that satisfies the condition $0 \le m \le 0$ is 0 from the Proposition 2.2.12c.   
Now let's suppose inductively that when $P(n)$ is true $P(m)$ is true for all natural numbers $m \le n$ and $P(n\pp)$ is true and that $P(n\pp)$ is true and we need to show that $P(m)$ is true for all natural numbers $m \le n\pp$. We know from the properties of $P$ that $P(n)$ is true when $P(n\pp)$ is true and from the inductive hypothesis that $P(n\pp)$ is also true thus $P(n)$ is true. Now that we know $P(n)$ is true we can show that $P(m)$ is true for all natural numbers $m \le n$ from the inductive hypothesis and we already know that $P(n\pp)$ is true thus proving that $P(m)$ is true for all natural numbers $m \le n\pp$ and closing the induction. ??
