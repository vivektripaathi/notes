# Asymptotic Notation Examples

#### Example 1: $f(n) = 2n^2 + 3n + 4$
$\Rightarrow 2n^2 + 3n + 4 \leq 2n^2 + 3n^2 + 4n^2$
$\Rightarrow 2n^2 + 3n + 4 \leq 9n^2$
$\Rightarrow f(n) = f(g(n)) = O(n^2)$

$\Rightarrow 2n^2 + 3n + 4 \geq 1*n^2$
$\Rightarrow \Omega(n^2)$

$\Rightarrow 1*n^2 \leq 2n^2 + 3n + 4 \leq 9n^2$
$\Rightarrow \theta(n^2)$


#### Example 2: $f(n) = n^2\log n + n$
$\Rightarrow 1*n^2\log n \leq n^2\log n + n \leq 10n^2\log n$
$\Rightarrow O(n^2\log n)$
$\Rightarrow \Omega(n^2\log n)$
$\Rightarrow \theta(n^2\log n)$

#### Example 3: $f(n) = n!$
$f(n) = n! = n*(n-1)*(n-2)*......*2*1$
$\Rightarrow 1*1*1....1*1 \leq 1*2*3*.....*n\leq n*n*n*.....*n$
$\Rightarrow 1 \leq 1*2*3*.....*n\leq n^n$
$\Rightarrow O(n^n)$
$\Rightarrow \Omega(1)$
$\Rightarrow \theta\to$Can't be found

#### Example 3: $f(n) = \log n!$
$\Rightarrow \log(1*1*1....1*1) \leq \log(1*2*3*.....*n)\leq \log(n*n*n*.....*n)$
$\Rightarrow 1 \leq log(1*2*3*.....*n)\leq \log n^n$
$\Rightarrow O(n\log n)$  $[\because \log n^n = n\log n]$
$\Rightarrow \Omega(1)$
