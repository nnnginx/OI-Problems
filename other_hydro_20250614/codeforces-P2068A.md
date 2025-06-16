## Description

<div><p>It is a municipality election year. Even though the leader of the country has not changed for two decades, the elections are always transparent and fair.</p><p>There are $n$ political candidates, numbered from $1$ to $n$, contesting the right to govern. The elections happen using a variation of the <span class="tex-font-style-underline">Ranked Voting System</span>. In their ballot, each voter will rank all $n$ candidates from most preferable to least preferable. That is, each vote is a permutation of $\{1, 2, \ldots, n\}$, where the first element of the permutation corresponds to the most preferable candidate.</p><p>We say that candidate $a$ defeats candidate $b$ if in more than half of the votes candidate $a$ is more preferable than candidate $b$.</p><p>As the election is fair and transparent, the state television has already decreed a list of $m$ facts！the $i$-th fact being "candidate $a_i$ has defeated candidate $b_i$"！all before the actual election!</p><p>You are in charge of the election commission and tallying up the votes. You need to present a list of votes that produces the outcome advertised on television, or to determine that it is not possible. However, you are strongly encouraged to find a solution, or you might upset higher-ups.</p></div><div class="input-specification"><p>The first line contains integers $n$ and $m$ ($2 \le n \le 50$, $1 \le m \le \frac{n(n-1)}{2}$)&nbsp;！ the number of parties and the number of pairs with known election outcomes.</p><p>The $i$-th of the following $m$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) ！ candidate $a_i$ defeats candidate $b_i$.</p><p>Each unordered pair $\{a_i, b_i\}$ is given at most once.</p></div><div class="output-specification"><p>Print $\texttt{YES}$ if there is a list of votes matching the facts advertised on television. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid list of votes, print one such list in the following lines.</p><p>Print the number $k$ of votes cast ($1 \le k \le 50\,000$). It can be shown that if there is a valid list of votes, there is one with at most $50\,000$ votes.</p><p>Then print $k$ lines. The $i$-th of these lines consists of a permutation of $\{1, 2, \ldots, n\}$ describing the $i$-th vote. The first number in the permutation is the most preferable candidate and the last one is the least preferable candidate.</p><p>For $1\le i\le m$, $a_i$ shall appear earlier than $b_i$ in more than $k{/}2$ of the $k$ permutations. For pairs of candidates $\{a, b\}$ not appearing in the election requirements list, the outcome can be arbitrary, including neither of $a$ and $b$ defeating the other.</p></div>

## Input

<p>The first line contains integers $n$ and $m$ ($2 \le n \le 50$, $1 \le m \le \frac{n(n-1)}{2}$)&nbsp;！ the number of parties and the number of pairs with known election outcomes.</p><p>The $i$-th of the following $m$ lines contains two integers $a_i$ and $b_i$ ($1 \le a_i, b_i \le n$, $a_i \ne b_i$) ！ candidate $a_i$ defeats candidate $b_i$.</p><p>Each unordered pair $\{a_i, b_i\}$ is given at most once.</p>

## Output

<p>Print $\texttt{YES}$ if there is a list of votes matching the facts advertised on television. Otherwise, print $\texttt{NO}$.</p><p>If there is a valid list of votes, print one such list in the following lines.</p><p>Print the number $k$ of votes cast ($1 \le k \le 50\,000$). It can be shown that if there is a valid list of votes, there is one with at most $50\,000$ votes.</p><p>Then print $k$ lines. The $i$-th of these lines consists of a permutation of $\{1, 2, \ldots, n\}$ describing the $i$-th vote. The first number in the permutation is the most preferable candidate and the last one is the least preferable candidate.</p><p>For $1\le i\le m$, $a_i$ shall appear earlier than $b_i$ in more than $k{/}2$ of the $k$ permutations. For pairs of candidates $\{a, b\}$ not appearing in the election requirements list, the outcome can be arbitrary, including neither of $a$ and $b$ defeating the other.</p>





```input1|
2 1
1 2
```




```input2|
3 3
1 2
2 3
3 1
```




```output1
YES
1
1 2
```




```output2
YES
3
1 2 3
2 3 1
3 1 2
```



## Note

<p>In the <span class="tex-font-style-bf">second sample</span>, Observe that candidate $1$ defeats candidate $2$ because it goes earlier in two out of three voters' permutations, which is more than half of all votes. Similarly, candidate $2$ defeats candidate $3$, and candidate $3$ defeats candidate $1$.</p>
