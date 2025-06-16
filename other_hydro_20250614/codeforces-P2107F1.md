## Description

<div><p><span class="tex-font-style-bf">This is the easy version of the problem. The difference between the versions is that in this version, $1\le n\le 5\cdot 10^3$ and you don't need to output the answer for each prefix. You can hack only if you solved all versions of this problem.</span></p><p>Leo works as a programmer in the city center, and his lover teaches at a high school in the suburbs. Every weekend, Leo would ride his bike to the suburbs to spend a nice weekend with his lover.</p><p>There are $n$ cyclists riding in front of Leo on this road right now. They are numbered $1$, $2$, $\ldots$, $n$ from front to back. Initially, Leo is behind the $n$-th cyclist. The $i$-th cyclist has an agility value $a_i$. </p><p>Leo wants to get ahead of the $1$-st cyclist. Leo can take the following actions as many times as he wants:</p><ul> <li> Assuming that the first person in front of Leo is cyclist $i$, he can go in front of cyclist $i$ for a cost of $a_i$. This puts him behind cyclist $i - 1$. </li><li> Using his super powers, swap $a_i$ and $a_j$ ($1\le i &lt; j\le n$) for a cost of $(j - i)$. </li></ul><p>Leo wants to know the minimum cost to get in front of the $1$-st cyclist. Here you only need to print the answer for the whole array, i.e. $[a_1, a_2, \ldots, a_n]$.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains a positive integer $n$ ($1 \leq n \leq 5\cdot 10^3$), representing the number of the cyclists.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot 10^3$.</p></div><div class="output-specification"><p>For each test case, print one integer representing the minimum cost for Leo to go from behind the $n$-th cyclist to in front of the $1$-st cyclist.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). The description of the test cases follows. </p><p>The first line of each test case contains a positive integer $n$ ($1 \leq n \leq 5\cdot 10^3$), representing the number of the cyclists.</p><p>The second line of each test case contains $n$ integers $a_1, \ldots, a_n$ ($1 \leq a_i \leq 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $5\cdot 10^3$.</p>

## Output

<p>For each test case, print one integer representing the minimum cost for Leo to go from behind the $n$-th cyclist to in front of the $1$-st cyclist.</p>





```input1|2,3,6,7
4
3
1 2 4
4
1 1 1 1
2
1 2
4
4 1 3 2
```




```output1
7
4
3
8
```



## Note

<p>In the first test case, one possible way to move from the position behind the $n$-th cyclist to the position in front of the $1$-st cyclist is:</p><ul> <li> Leo swaps $a_2$ $(i=2)$ and $a_3$ $(j=3)$, then the array becomes $[1,4,2]$; it costs $j-i=3-2=1$.</li><li> Leo is behind the $3$-rd cyclist and moves behind the $2$-nd cyclist; it costs $a_3=2$.</li><li> Leo swaps $a_1$ $(i=1)$ and $a_2$ $(j=2)$, then the array becomes $[4,1,2]$; it costs $j-i=2-1=1$.</li><li> Leo is behind the $2$-nd cyclist and moves behind the $1$-st cyclist; it costs $a_2=1$.</li><li> Leo swaps $a_1$ $(i=1)$ and $a_2$ $(j=2)$, then the array becomes $[1,4,2]$; it costs $j-i=2-1=1$.</li><li> Leo moves ahead of the $1$-st cyclist; it costs $a_1=1$.</li></ul> <p>So the total cost is $1+2+1+1+1+1=7$. It can be proved that $7$ is the minimum cost.</p><p>In the second test case, to move ahead of the $1$-st cyclist from the position behind the $n$-th cyclist, Leo should not swap anyone's agility value. The total cost is $1+1+1+1=4$.</p>
