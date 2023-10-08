# Algorithm
A step-by-step procedure for solving a computational problem.

# Algorithm Analysis
Theoretical estimation of the required resources of an algorithm to solve a specific computational problem. 
Analysis of algorithms is the determination of the amount of time and space resources required to execute it.

## Why it is important?
- Behaviour prediction without implementation.
- The idea is to measure order of growth.
- More importantly, by analysing different algorithms, we can compare them to determine the best one for our purpose.

## Types of Case Analysis:
1.  Best case
2.  Worst case
3.  Average case

# Asymptotic Analysis
In asymptotic analysis, we evaluate the performance of an algorithm in terms of input size(we don't measure the actual running time).
- We calculate how the time(or space) taken by an algorithm increases with the input size.

# Order of Growth
A function $f(n)$ is said to be growing faster than $g(n)$ if
$$lim_{n \to \infty}\frac{g(n)}{f(n)} = 0$$
OR 
$$lim_{n \to \infty}\frac{f(n)}{g(n)} = \infty$$

- $f(n)$ and $g(n)$ represents time taken by the algorithm.
- $n, \ f(n), \ g(n)$ $\geq$ 0.

## Direct way to Find and Compare Growths
1.  Ignore Lower Order Terms.
2. Ignore leading Term Constant
Example:
$f(n)  = 2n^2 + n + 6$,    Order of Growth : $n^2$ Quadratic
$g(n) = 100n +3$         Order of Growth : $n$ Linear.

#### How do we compare terms?

$$C < \log\log n < \log n < n^\frac 1 3 < n^\frac 1 2 < n < n^2 < n^3 < 2^n < n^n$$

# Asymptotic Notation :

## Big-oh(O) Notation:
The function $f(n) = O(g(n)) \ iff\ \exists$ +ve constants C and $n_0$ such that $f(n) \leq C * g(n) \ \forall \ n \geq n_0$.

## Omega($\Omega$) Notation:
The function $f(n) = O(g(n)) \ iff\ \exists$ +ve constants C and $n_0$ such that $f(n) \geq C * g(n) \ \forall \ n \geq n_0$

## Theta($\theta$) Notation:
The function $f(n) = O(g(n)) \ iff\ \exists$ +ve constants $C_1, C_2$ and $n_0$ such that $C_1*g(n)\leq f(n) \leq C_2 * g(n) \ \forall \ n \geq n_0$



