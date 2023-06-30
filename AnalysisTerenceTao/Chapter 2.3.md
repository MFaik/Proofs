##### Definition of Multiplication of Natural Numbers
$0 \times m := 0$
$\newcommand{\pp}{\verb!++!}$$(n\pp) \times m := (n \times m) + m$ 
##### Lemma 2.3.1a
$m \times 0 = 0$
We'll induct on $n$. The base case $0 \times 0 = 0$ from the definition of multiplication. We'll inductively assume that $n \times 0 = 0$  and prove that $(n\pp) \times 0 = 0$. From the definition of multiplication $(n\pp) \times 0$ is equivalent to $(n \times 0) + 0$. We already know that $n \times 0 = 0$ from the inductive hypothesis so we can see that $(n\pp) \times 0 = 0$.  $\square$
##### Lemma 2.3.1b
$n \times (m\pp) = n \times m + n$ 
We'll induct on n. The base case is $0 \times (m\pp) = 0 \times m + 0$. We can use the definition of multiplication to show that both of them are equal to 0. Now we'll inductively assume that $n \times (m\pp) = n \times m + n$ and prove $(n\pp) \times (m\pp) = (n\pp) \times m + (n\pp)$.
The right-hand side of the equation is equal to $n \times m + m + (n\pp)$ from the definition of multiplication.
The left-hand side of the equation is equal to $n \times (m\pp) + (m\pp)$ from the definition of multiplication and this is equal $n \times m + n + (m\pp)$ and we can rewrite this as $n \times m + m + (n\pp)$ to see that it is indeed equal to the right-hand side and close the induction. $\square$
##### Lemma 2.3.2
$n \times m = m \times n$
We'll induct on $n$. First we'll prove the base case $n = 0$. We know that $0 \times m = 0$ from the definition of multiplication and we know that $m \times 0 = 0$ from Lemma 2.3.1a thus we have proven the base case. We will inductively assume $n \times m = m \times n$ and need to prove that  $(n\pp) \times m = m \times (n\pp)$. 
The left-hand side is $n \times m + m$ from the definition of multiplication.
The right-hand side is $m \times n + m$ from Lemma 2.3.1b and from the inductive hypothesis this is equal to $n \times m + m$ which is the same as the left-hand side thus closing the induction. $\square$ 
##### Lemma 2.3.3
Let $n$,$m$ be natural numbers. Then $n \times m = 0$ iff at least one of them is equal to zero.
We know from the definition of multiplication and Lemma 2.3.1a that if at least one of $n$ and $m$ is 0, then $n \times m = 0$.
For the sake of contradiction we'll assume that $n \times m = 0$ and both $n$ and $m$ are positive numbers. We know that if n is positive there exists a natural number $c$ such that $c\pp = n$, and we'll rewrite the equation as $(c\pp) \times m = 0$. From the definition of multiplication we know that $(c++) \times m = c \times m + m$. So the equation becomes $c \times m + m = 0$. It doesn't really matter if $c \times m$ is zero or not because we know that a natural number plus a positive number is never zero. This contradiction implies that if $n \times m = 0$ then at least one of $n$ and $m$ must be zero thus completing the proof. $\square$
##### Proposition 2.3.4
$a(b + c) = ab + ac$
##### Proposition 2.3.5
$(a \times b) \times c = a \times (b \times c)$
We keep $a$ and $c$ fixed and use induction on $b$. The base case $b = 0$ is simple to prove. $(a \times 0) \times c$ is zero by the definition of multiplication and Lemma 2.3.1a, and we can use the same logic to see that $a \times (0 \times c)$ is also zero.
Now we'll inductively assume that $(a \times b) \times c = a \times (b \times c)$ and prove that $(a \times (b\pp)) \times c = a \times ((b\pp) \times c)$. 
We can follow these steps to rewrite the left-hand side:
$(a \times (b\pp)) \times c = (a \times b + a) \times c$ from Lemma 2.3.1b
$(a \times b + a) \times c = (a \times b) \times c + a \times c$ from Proposition 2.3.5
$(a \times b) \times c + a \times c = a \times (b \times c) + a \times c$ from the inductive hypothesis
Similarly we can rewrite the right-hand side as:
$a \times ((b\pp) \times c) = a \times (b \times c + c)$ from the definition of multiplication
$a \times (b \times c + c) = a \times (b \times c) + a \times c$ from Proposition 2.3.4
and we can see that this is the same as the left-hand side thus completing the proof $\square$ 
##### Proposition 2.3.6
If $a$, $b$ are natural numbers such that $a < b$, and c is positive, then $ac < bc$
##### Corollary 2.3.7
If $ac = bc$ and c is non-zero, then $a = b$
##### Proposition 2.3.9
We'll use induction on $n$. The base case is easy to show because $m = 0$ and $r = 0$ satisfies the conditions. Now let's inductively assume that there exists natural numbers $m$ and $r$ such that $0 \le r < q$ and $n = mq + r$. We need to prove that there exists natural numbers $m'$ and $r'$ such that $0 \le r' < q$ and $n\pp = m'q + r'$. I'll split this into two cases. Where $r\pp = q$ and $r\pp < q$. We know that $r\pp \le q$ because $r < q$ thus we don't need to look at the case where $r\pp > q$.
First the case where $r\pp < q$. We can just say $m' = m$ and $r' = r\pp$ and this will satisfy the conditions.
Second the case where $r\pp = q$. We cannot just say that $r' = r\pp$ because that would contradict the condition $r' < q$. Even if it doesn't fit that condition we know that this equation still holds: $n\pp = mq + r\pp$ and because we know that $r\pp=q$ we can write $n\pp = mq + q = (m\pp)q + 0$ which satisfies all the conditions. So in this second case we can say that such $m$ and $n$ exists and they are $m' = m\pp$ and $r' = 0$. This closes the induction and finishes the proof $\square$   
##### Definition 2.3.11
$m^0 := 1$
$m^{n\pp} = m^n \times m$ 
##### Exercise 2.3.4
Prove $(a + b)^2 = a^2 + 2ab + b^2$
We can rewrite the statement without the exponents by using the definition of the exponents:
$(a+b)(a+b) = aa + 2ab + bb$
$(a+b)(a+b) = a \times (a + b) + b \times (a + b) = aa + ab + ba + bb$ from Proposition 2.3.4
$aa + ab + ba + bb = aa + ba + ba + bb$ from Lemma 2.3.2.
$aa + ba + ba + bb = aa + 2ba + bb$ from the definition of multiplication and now we can see that the left side is equal to the right side. $\square$