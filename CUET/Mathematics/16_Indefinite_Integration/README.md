Integration is the reverse process of differentiation also known as anto-derivate.
$\int f(x) = F(x) + C$
$f(x)\to Integrand$
$F(x)\to Integral$
$x\to Variable\ of\ Integration$
$C \to Constant$
- The concept of integration originated during the course of finding area of plane figure.

| $\int dx$                      | x + C                              |
| ------------------------------ | ---------------------------------- |
| $\int x^n dx$                  | $\frac{x^{n+1}}{n+1}$ + C $n\neq1$ |
| $\int cosx$                    | sinx + C                           |
| $\int sinx$                    | -cosx + C                          |
| $\int sec^2x$                  | tanx + C                           |
| $\int cosec^2x$                | -cotx + C                          |
| $\int secxtanx$                | secx + C                           |
| $\int cosecxcotx$              | -cosecx + C                        |
| $\int \frac{dx}{\sqrt{1-x^2}}$ | $sin^{-1}x$ + C                    |
| $\int \frac{dx}{\sqrt{1-x^2}}$ | $-cos^{-1}x$ + C                   |
| $\int \frac{dx}{1+x^2}$        | $tan^{-1}x$ + C                    |
| $\int \frac{dx}{1+x^2}$        | $-cot^{-1}x$ + C                   |
| $\int\frac{dx}{x\sqrt{x^2-1}}$ | $sec^-1x$ + C                      |
| $\int\frac{dx}{x\sqrt{x^2-1}}$ | $-cosec^-1x$ + C                   |
| $\int e^x dx$                  | $e^x$ + C                          |
| $\int \frac{1}{x}dx$           | logx + C                           |
| $\int  a^x$dx                  | $\frac{a^x}{\log a}$                                   |
- $\int$ tanx dx = log|sec x| + C
- $\int$ cot x dx = log|sin x| + C
- $\int$ sec x dx = log|sec x + tan x| +C
- $\int$ cosec x dx = log|cosec x + cot x| + C

## Theorems of Integration
1. $\int\ f(x) dx = k\int\ f(x) dx$, where k is a constant.
2. $\int\{f_1(x) \pm \int f_2(x) \pm \int f_3(x)\} = \int f_1(x) \pm \int f_2(x) \pm \int f_3(x)$
3. $\int f(ax\pm b) =  \frac 1 a F(ax \pm b)$

### Forms 
1. $\int \frac{dx}{quadratic}$
- $\int \frac{1}{x^2-a^2} = \frac{1}{2a}log|\frac{x-a}{x+a}|$ 
- $\int \frac{1}{a^2-x^2} = \frac{1}{2a}log|\frac{a+x}{a-x}|$ 
- $\int\frac{dx}{a^2+x^2} = \frac 1 2 tan^{-1}\frac x a + C$
- $\int \frac{dx}{\sqrt{a^2+x^2}} = log(x + \sqrt{x^2 + a^2}) + C$
- $\int \frac{dx}{\sqrt{a^2-x^2}} = sin^{-1}\frac x a + C$
- $\int \frac{dx}{\sqrt{x^2-a^2}} = log_e|x + \sqrt{x^2-a^2}|$

# Methods of Integration
1. By substitution
2. By using partial function
3. By Parts
 
## Substitution Method
the following are the 3 important consequences.
1. $\int (f(x))^nf'(x)= \frac{(f(x))^{n+1}}{n+1}+C, \ where\ n\neq0$ 
2. $\int \frac{f'(x)}{f(x)}dx = log_e|f(x)|+C$
3. $\int\frac{f'(x)}{\sqrt{f(x)}}dx = 2\sqrt{f(x)} + C$

## Partial Fraction
$\frac{1}{(ax+b)(cx+d)} = \frac{A}{ax+b} + \frac{B}{cx+b}$
$\frac{1}{(ax+b)(cx+d)^2} = \frac{A}{ax+b}+\frac{B}{cx+b}+\frac{B}{(cx+b)^2}$
$\frac{1}{(ax+b)(c^2x^2+d)} = \frac{A}{ax+b} + \frac{cx+d}{cx^2+d}$

## By Parts
$\int f(x).g(x)dx$
$f(x)\int g(x)dx-\int(f'(x)\int g(x)dx) dx$

#### Priority to decide $I^{st} f^n$ over $II^{nd} f^n$
I - Inverse Function
L - Logartmic Function
A - Algebric Function
T - Trigonometric Function
E - Exponential Function
- If not from anyu of the above function then, $II^{nd} f^n$ is $f^n$ whose integration is known or simple.

#### Formula #kahi_ye_vo_to_nhi
- $\int e^x[f(x)+f'(x)]dx = e^xf(x)+C$
- $\int xf'(x)+f(x)dx = xf(x) + C$

- $\int \sqrt{x^2 + a^2} dx = \frac x 2\sqrt{x^2+a^2} + \frac{a^2}{2}log(x+\sqrt{x^2+a^2}+C)$
- $\int \sqrt{x^2 + a^2} dx = \frac x 2\sqrt{x^2+a^2} - \frac{a^2}{2}log(x+\sqrt{x^2+a^2}+C)$
- $\int \sqrt{a^2-x^2} dx = \frac x 2\sqrt{a^2-x^2} + \frac{a^2}{2}sin^-1\frac x a +C$
