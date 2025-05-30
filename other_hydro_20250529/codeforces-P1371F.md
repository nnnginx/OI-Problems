## Description

<div><p>You are a warrior fighting against the machine god Thor.</p><p>Thor challenge you to solve the following problem:</p><p>There are $n$ conveyors arranged in a line numbered with integers from $1$ to $n$ from left to right. Each conveyor has a symbol "<span class="tex-font-style-tt">&lt;</span>" or "<span class="tex-font-style-tt">&gt;</span>". The initial state of the conveyor $i$ is equal to the $i$-th character of the string $s$. There are $n+1$ holes numbered with integers from $0$ to $n$. The hole $0$ is on the left side of the conveyor $1$, and for all $i \geq 1$ the hole $i$ is on the right side of the conveyor $i$.</p><p>When a ball is on the conveyor $i$, the ball moves by the next rules:</p><p>If the symbol "<span class="tex-font-style-tt">&lt;</span>" is on the conveyor $i$, then:</p><ul> <li> If $i=1$, the ball falls into the hole $0$. </li><li> If the symbol "<span class="tex-font-style-tt">&lt;</span>" is on the conveyor $i-1$, the ball moves to the conveyor $i-1$. </li><li> If the symbol "<span class="tex-font-style-tt">&gt;</span>" is on the conveyor $i-1$, the ball falls into the hole $i-1$. </li></ul><p>If the symbol "<span class="tex-font-style-tt">&gt;</span>" is on the conveyor $i$, then:</p><ul> <li> If $i=n$, the ball falls into the hole $n$. </li><li> If the symbol "<span class="tex-font-style-tt">&gt;</span>" is on the conveyor $i+1$, the ball moves to the conveyor $i+1$. </li><li> If the symbol "<span class="tex-font-style-tt">&lt;</span>" is on the conveyor $i+1$, the ball falls into the hole $i$. </li></ul><p>You should answer next $q$ queries, each query is defined by the pair of integers $l, r$ ($1 \leq l \leq r \leq n$): </p><ul> <li> First, for all conveyors $l,l+1,...,r$, the symbol "<span class="tex-font-style-tt">&lt;</span>" changes to "<span class="tex-font-style-tt">&gt;</span>" and vice versa. <span class="tex-font-style-bf">These changes remain for the next queries.</span> </li><li> After that, put <span class="tex-font-style-bf">one ball</span> on each conveyor $l,l+1,...,r$. Then, each ball falls into some hole. Find the maximum number of balls in one hole. <span class="tex-font-style-bf">After the query all balls disappear and don't considered in the next queries.</span> </li></ul></div><div class="input-specification"><p>The first line contains two integers $n$, $q$ ($1 \le n \le 5 \times 10^5 , 1 \le q \le 10^5$).</p><p>The second line contains a string $s$ of length $n$. It consists of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>". </p><p>Next $q$ lines contain the descriptions of the queries, $i$-th of them contains two integers $l$, $r$ $(1 \le l \le r \le n)$, describing the $i$-th query.</p></div><div class="output-specification"><p>Print $q$ lines, in the $i$-th of them print the answer to the $i$-th query.</p></div>

## Input

<p>The first line contains two integers $n$, $q$ ($1 \le n \le 5 \times 10^5 , 1 \le q \le 10^5$).</p><p>The second line contains a string $s$ of length $n$. It consists of characters "<span class="tex-font-style-tt">&lt;</span>" and "<span class="tex-font-style-tt">&gt;</span>". </p><p>Next $q$ lines contain the descriptions of the queries, $i$-th of them contains two integers $l$, $r$ $(1 \le l \le r \le n)$, describing the $i$-th query.</p>

## Output

<p>Print $q$ lines, in the $i$-th of them print the answer to the $i$-th query.</p>

## Samples

```input1
5 6
&gt;&lt;&gt;&gt;&lt;
2 4
3 5
1 5
1 3
2 4
1 5
```

```output1
3
3
5
3
2
3
```




## Note

<ul> <li> In the first query, the conveyors change to "<span class="tex-font-style-tt">&gt;&gt;&lt;&lt;&lt;</span>". After that, put a ball on each conveyor $\{2,3,4\}$. All three balls fall into the hole $2$. So the answer is $3$. </li><li> In the second query, the conveyors change to "<span class="tex-font-style-tt">&gt;&gt;&gt;&gt;&gt;</span>". After that, put a ball on each conveyor $\{3,4,5\}$. All three balls fall into the hole $5$. So the answer is $3$. </li><li> In the third query, the conveyors change to "<span class="tex-font-style-tt">&lt;&lt;&lt;&lt;&lt;</span>". After that, put a ball on each conveyor $\{1,2,3,4,5\}$. All five balls fall into the hole $0$. So the answer is $5$. </li><li> In the fourth query, the conveyors change to "<span class="tex-font-style-tt">&gt;&gt;&gt;&lt;&lt;</span>". After that, put a ball on each conveyor $\{1,2,3\}$. All three balls fall into the hole $3$. So the answer is $3$. </li><li> In the fifth query, the conveyors change to "<span class="tex-font-style-tt">&gt;&lt;&lt;&gt;&lt;</span>". After that, put a ball on each conveyor $\{2,3,4\}$. Two balls fall into the hole $1$, and one ball falls into the hole $4$. So, the answer is $2$. </li><li> In the sixth query, the conveyors change to "<span class="tex-font-style-tt">&lt;&gt;&gt;&lt;&gt;</span>". After that, put a ball on each conveyor $\{1,2,3,4,5\}$. Three balls fall into the hole $3$, one ball falls into the hole $0$ and one ball falls into the hole $5$. So, the answer is $3$. </li></ul>
