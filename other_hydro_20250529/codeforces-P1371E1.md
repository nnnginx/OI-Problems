## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between versions is the constraints on $n$ and $a_i$. You can make hacks only if all versions of the problem are solved.</span></p><p>First, Aoi came up with the following idea for the competitive programming problem:</p><p>Yuzu is a girl who collecting candies. Originally, she has $x$ candies. There are also $n$ enemies numbered with integers from $1$ to $n$. Enemy $i$ has $a_i$ candies.</p><p>Yuzu is going to determine a permutation $P$. A permutation is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $\{2,3,1,5,4\}$ is a permutation, but $\{1,2,2\}$ is not a permutation ($2$ appears twice in the array) and $\{1,3,4\}$ is also not a permutation (because $n=3$ but there is the number $4$ in the array).</p><p>After that, she will do $n$ duels with the enemies with the following rules:</p><ul> <li> If Yuzu has <span class="tex-font-style-bf">equal or more</span> number of candies than enemy $P_i$, she wins the duel and <span class="tex-font-style-bf">gets $1$ candy</span>. Otherwise, she loses the duel and gets nothing. </li><li> The candy which Yuzu gets will be used in the next duels. </li></ul><p>Yuzu wants to <span class="tex-font-style-bf">win all duels</span>. How many valid permutations $P$ exist?</p><p>This problem was easy and wasn't interesting for Akari, who is a friend of Aoi. And Akari made the following problem from the above idea:</p><p>Let's define $f(x)$ as the number of valid permutations for the integer $x$.</p><p>You are given $n$, $a$ and <span class="tex-font-style-bf">a prime number</span> $p \le n$. Let's call a positive integer $x$ <span class="tex-font-style-bf">good</span>, if the value $f(x)$ is <span class="tex-font-style-bf">not</span> divisible by $p$. Find <span class="tex-font-style-bf">all</span> good integers $x$.</p><p>Your task is to solve this problem made by Akari.</p></div><div class="input-specification"><p>The first line contains two integers $n$, $p$ $(2 \le p \le n \le 2000)$. It is guaranteed, that the number $p$ is prime (it has exactly two divisors $1$ and $p$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(1 \le a_i \le 2000)$.</p></div><div class="output-specification"><p>In the first line, print the number of good integers $x$.</p><p>In the second line, output all good integers $x$ <span class="tex-font-style-bf">in the ascending order</span>.</p><p>It is guaranteed that the number of good integers $x$ does not exceed $10^5$.</p></div>

## Input

<p>The first line contains two integers $n$, $p$ $(2 \le p \le n \le 2000)$. It is guaranteed, that the number $p$ is prime (it has exactly two divisors $1$ and $p$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ $(1 \le a_i \le 2000)$.</p>

## Output

<p>In the first line, print the number of good integers $x$.</p><p>In the second line, output all good integers $x$ <span class="tex-font-style-bf">in the ascending order</span>.</p><p>It is guaranteed that the number of good integers $x$ does not exceed $10^5$.</p>

## Samples

```input1
3 2
3 4 5
```

```output1
1
3
```






```input2
4 3
2 3 5 6
```

```output2
2
3 4
```






```input3
4 3
9 1 1 1
```

```output3
0
```




## Note

<p>In the first test, $p=2$.</p><ul> <li> If $x \le 2$, there are no valid permutations for Yuzu. So $f(x)=0$ for all $x \le 2$. The number $0$ is divisible by $2$, so all integers $x \leq 2$ are not good. </li><li> If $x = 3$, $\{1,2,3\}$ is the only valid permutation for Yuzu. So $f(3)=1$, so the number $3$ is good. </li><li> If $x = 4$, $\{1,2,3\} , \{1,3,2\} , \{2,1,3\} , \{2,3,1\}$ are all valid permutations for Yuzu. So $f(4)=4$, so the number $4$ is not good. </li><li> If $x \ge 5$, all $6$ permutations are valid for Yuzu. So $f(x)=6$ for all $x \ge 5$, so all integers $x \ge 5$ are not good. </li></ul><p>So, the only good number is $3$.</p><p>In the third test, for all positive integers $x$ the value $f(x)$ is divisible by $p = 3$.</p>
