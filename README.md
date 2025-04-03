# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

## Big O describes an upper bound while little o describes a strict upper bound

So in the case of Big O, if f(n) = O(g(n)) then f(n) grows no faster than g(n)

In the case of little o, if f(n) = O(g(n)) then f(n) grows strictly slower than g(n)

# Proof:

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

If the definition of Big O is $f(n)\in O(g(n)) \iff \exists c>0 ∧ \exists n_0, \forall n\ge n_0: f(n) n\le c g(n)$

that means there needs to be a single positive constant c that must be true and  f(n) can be less than or equal to g(n). 

Little o needs all positive constant c's to be true and f(n) should be less than c g(n)


Sources: 
[here](https://www.stat.cmu.edu/~cshalizi/uADA/13/lectures/app-b.pdf#:~:text=Big-O%20means%20“is%20of%20the%20same%20order,(n)%20=%20o(1)%2C%20or%20g(n)/f%20(n)%20!)

and [here at The Algebra of Big O](https://www.cs.odu.edu/~zeil/cs361/sum24/Public/algebra/index.html#the-tao-of-n)

and [discrete math cheat sheet](https://www.compscilib.com/cheatsheets/discrete-math)
