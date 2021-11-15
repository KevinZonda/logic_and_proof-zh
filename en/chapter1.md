# Introduction

> Source: <https://leanprover.github.io/logic_and_proof/introduction.html>  
> Licensed under Apache 2.0


## Mathematical Proof

Although there is written evidence of mathematical activity in Egypt as early as 3000 BC, many scholars locate the birth of mathematics proper in ancient Greece around the sixth century BC, when deductive proof was first introduced. Aristotle credited Thales of Miletus with recognizing the importance of not just what we know but how we know it, and finding grounds for knowledge in the deductive method. Around 300 BC, Euclid codified a deductive approach to geometry in his treatise, the *Elements*. Through the centuries, Euclid’s axiomatic style was held as a paradigm of rigorous argumentation, not just in mathematics, but in philosophy and the sciences as well.

Here is an example of an ordinary proof, in contemporary mathematical language. It establishes a fact that was known to the Pythagoreans.

---

**Theorem.** $\sqrt{2}$ is irrational, which is to say, it cannot be expressed as a fraction $a/b$, where $a$ and $b$ are integers.

**Proof.** Suppose $\sqrt{2}=a/b$ for some pair of integers $a$ and $b$. By removing any common factors, we can assume $a/b$ is in lowest terms, so that $a$ and $b$ have no factor in common. Then we have $a=\sqrt{2}b$, and squaring both sides, we have $a^2=2b^2$.

The last equation implies that $a^2$ is even, and since the square of an odd number is odd, $a$ itself must be even as well. We therefore have $a=2c$ for some integer $c$. Substituting this into the equation $a^2=2b^2$, we have $4c^2=2b^2$, and hence $2c^2=b^2$. This means that $b^2$ is even, and so $b$ is even as well.

The fact that $a$ and $b$ are both even contradicts the fact that $a$ and $b$ have no common factor. So the original assumption that $\sqrt{2}=a/b$ is false.

---


In the next example, we focus on the natural numbers,

$$
N=\left\{0,1,2,\cdots\right\}.
$$

A natural number $n$ greater than or equal to 2 is said to be *composite* if it can be written as a product $n=m\cdot k$ where neither $m$ nor $k$ is equal to $1$, and *prime* otherwise. Notice that if $n=m\cdot k$ witnesses the fact that $n$ is composite, then $m$ and $k$ are both smaller than $n$. Notice also that, by convention, 0 and 1 are considered neither prime nor composite.

---

**Theorem.** Every natural number greater than or equal to 2 can be written as a product of primes.

**Proof.** We proceed by induction on $n$. Let $n$ be any natural number greater than 2. If $n$ is prime, we are done; we can consider $n$ itself as a product with one term. Otherwise, $n$ is composite, and we can write $n=m\cdot k$ where $m$ and $k$ are smaller than $n$ and greater than 1. By the inductive hypothesis, each of m and k can be written as a product of primes, say $m=p_1\cdot p_2\cdot \cdots \cdot p_u$ and $k=q_1\cdot q_2\cdot \cdots \cdot q_v$. But then we have

$$
n=m\cdot k=p_1 \cdot p_2\cdot \cdots \cdot p_u \cdot q_1 \cdot q_2\cdot \cdots \cdot q_v,
$$

a product of primes, as required.

---

Later, we will see that more is true: every natural number greater than 2 can be written as a product of primes in a unique way, a fact known as the *fundamental theorem of arithmetic*.

The first goal of this course is to teach you to write clear, readable mathematical proofs. We will do this by considering a number of examples, but also by taking a reflective point of view: we will carefully study the components of mathematical language and the structure of mathematical proofs, in order to gain a better understanding of how they work.