## 题目描述
For a positive integer $k$, Euler's totient function $\phi(k)$ is defined as the number of positive integers less than or equal to $k$ and relatively prime to $k$.
For example, $\phi(9) = 6$, $\phi(24) = 8,$ and $\phi(1) = 1$. (As a reminder, the greatest common divisor (gcd) of two positive integers $a$ and $b$ is the greatest positive integer that divides both $a$ and $b$. Two positive integers are relatively prime if their gcd is $1$.)

Euler's product formula gives the value of $\phi(k)$ in terms of the prime factorization of $k$. For a prime $p$, let $\nu_p(k)$ be the highest power of $p$ which divides $k$ (so for example, $\nu_2(48) = 4$, $\nu_3(48)=1$, and $\nu_5(48)=0$). If $k$ is a product of powers of prime factors, $k = \prod_{i=1}^j p_i^{\nu_{p_i}(k)}$ (where the product only includes primes $p_i$ with $\nu_{p_i}(k) > 0$), 
then 
$$ \phi(k) = \prod_{i=1}^j \left[(p_i - 1)\left(p_i^{\nu_{p_i}(k)-1}\right)\right].$$

A recent edition of The American Mathematical Monthly (Li et al., *Positive Rational Numbers of the Form $\phi(m^2)/\phi(n^2)$*, 128(2), 2021) proved the following fact about totient quotients: for any pair of positive integers $a$, $b$ there is a unique pair of positive integers $m$, $n$ for which:
- $\frac{a}{b} = \frac{\phi(m^2)}{\phi(n^2)};$
- if a prime $p$ divides the product $mn$, then $\nu_p(m) \neq \nu_{p}(n)$;
- $\gcd(m,n)$ is square-free: that is, for every prime $p$, $\gcd(m,n)$ is not divisible by $p^2$.

Conditions 2 and 3 guarantee that $m$ and $n$ are the unique smallest pair of positive integers satisfying condition 1.

You'd like to verify this claim numerically. Write a program which takes as input two integers $a$ and $b$ and outputs the corresponding pair $m, n$.

## 输入格式
The only line of input contains two space-separated integers $a$ and $b$ ($ 1 \leq a, b \leq 10\,000$). These two integers are guaranteed to be relatively prime. Additionally, $a$ and $b$ will be chosen so that output values $m$ and $n$ are less than $2^{63}$.

## 输出格式
Print the two positive integers $m$ and $n$ satisfying all three of the conditions of The American Mathematical Monthly's theorem, separated by a space. It is guaranteed that $ m, n < 2^{63}$.

```input1
9 13
```

```output1
18 13
```

```input2
19 47
```

```output2
13110 18612
```

