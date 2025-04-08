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

Little o requires the inequality to hold for all positive constants c,

while bigO only requires it to hold for some constant c.

1. Recall definitions:
   
   Little-o notation:$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

   So for all values of $c > 0$, there is some threshold $n_0$ where for all $n\ge n_0$, $f(n) < c g(n)$ 

   Big-O notation:$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) \le c g(n)$

   So there is at least one value of $c > 0$ where there's some value $n_0$ where for all $n\ge n_0$ $f(n) \le c g(n)$
   
2. Assuming f(n) is within o(g(n)) the little-o condition is true.
   
3. Since little-o says any positive c works, let c = 1 .
   
4. With c = 1, little-o guarantees some threshold $n_0$ such that for all n >= $n_0$,
   $|f(n)| < |g(n)|$
   
5. So if $|f(n)| < |g(n)|$ then $|f(n)| <= |g(n)|$
    
6. This means a specific value of c (in this case 1) that satisfies the big-O definition.
    
7. Therefore, $f(n) \in o(g(n)) implies f(n) \in O(g(n))$

Q.E.D.

Sources: 
[here](https://www.stat.cmu.edu/~cshalizi/uADA/13/lectures/app-b.pdf#:~:text=Big-O%20means%20“is%20of%20the%20same%20order,(n)%20=%20o(1)%2C%20or%20g(n)/f%20(n)%20!)

and [here at The Algebra of Big O](https://www.cs.odu.edu/~zeil/cs361/sum24/Public/algebra/index.html#the-tao-of-n)

and [discrete math cheat sheet](https://www.compscilib.com/cheatsheets/discrete-math)

and [asymptotic notation for little-o and big-o](https://stackoverflow.com/questions/1364444/difference-between-big-o-and-little-o-notation)

# Plagiarism Statement

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
