[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/fbkbKZ5N)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$

Answer: 

$T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot (\log_{5} n) \forall n \geq n_0$\
= $T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot \frac{(\log_{2} n)} {(\log_{2} 5)} \forall n \geq n_0$\
$\log_{2} 5 = d$ where d is a constant.\ 
= $T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot \frac{(\log_{2} n)} {c} \forall n \geq n_0$\
= $T(n) \in O(\log_{5} n) \iff \exists c, n_0: T(n) \leq c \cdot \frac {1} {d} \cdot (\log_{2} n) \forall n \geq n_0$\
$T(n) \in O(\log_{5} n) \iff T(n) \in O(\log_{2} n)
