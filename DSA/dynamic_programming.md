1. What is Dynamic Programming?
Dynamic Programming is an algorithm design technique that solves a complex problem by breaking it into smaller subproblems and storing their results so that we don't calculate the same subproblem repeatedly.

Let's understand this with an example.

Suppose you want to calculate the 5th Fibonacci number.

The Fibonacci sequence is:
\[
0,1,1,2,3,5,8,13,\ldots
\]

The mathematical formula is:
\[
F(n)=F(n-1)+F(n-2)
\]

Therefore:
\[
F(5)=F(4)+F(3)
\]

And:
\[
F(4)=F(3)+F(2)
\]

Notice something?

We calculate \(F(3)\) more than once.

This is unnecessary repeated work.