## Description

<div><p> </p><center><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small"><span class="tex-font-style-it">At his orange orchard, Florida Man receives yet another spam letter, delivered by a crow. Naturally, he's sending it back in the most inconvenient manner possible.</span></span></td></tr></tbody></table></center><p>A crow is sitting at position $0$ of the number line. There are $n$ scarecrows positioned at integer coordinates $a_1, a_2, \ldots, a_n$ along the number line. These scarecrows have been enchanted, allowing them to move left and right at a speed of $1$ unit per second.</p><p>The crow is afraid of scarecrows and wants to stay at least a distance of $k$ ahead of the nearest scarecrow positioned <span class="tex-font-style-bf">at or before</span> it. To do so, the crow uses its teleportation ability as follows:</p><ul> <li> Let $x$ be the current position of the crow, and let $y$ be the largest position of a scarecrow such that $y \le x$. If $x - y &lt; k$, meaning the scarecrow is too close, the crow will instantly teleport to position $y + k$. </li></ul><p>This teleportation happens instantly and continuously. The crow will keep checking for scarecrows positioned at or to the left of him and teleport whenever one gets too close (which could happen at non-integral times). Note that besides this teleportation ability, the crow will not move on its own.</p><p>Your task is to determine the minimum time required to make the crow teleport to a position greater than or equal to $\ell$, assuming the scarecrows move optimally to allow the crow to reach its goal. For convenience, you are asked to output <span class="tex-font-style-bf">twice the minimum time</span> needed for the crow to reach the target position $\ell$. It can be proven that this value will always be an integer.</p><p>Note that the scarecrows can start, stop, or change direction at any time (possibly at non-integral times).</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n, k, \ell$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq \ell \leq 10^8$)&nbsp;�� the number of scarecrows, the teleportation distance, and the target position of the crow, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq \ell$)&nbsp;�� the initial positions of the $n$ scarecrows.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p></div><div class="output-specification"><p>For each test case, output a single integer representing the <span class="tex-font-style-bf">twice the minimum time</span> required for the crow to teleport to a position greater than or equal to $\ell$.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains three integers $n, k, \ell$ ($1 \leq n \leq 2 \cdot 10^5$, $1 \leq k \leq \ell \leq 10^8$)&nbsp;�� the number of scarecrows, the teleportation distance, and the target position of the crow, respectively.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \leq a_1 \leq a_2 \leq \ldots \leq a_n \leq \ell$)&nbsp;�� the initial positions of the $n$ scarecrows.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $2 \cdot 10^5$. </p>

## Output

<p>For each test case, output a single integer representing the <span class="tex-font-style-bf">twice the minimum time</span> required for the crow to teleport to a position greater than or equal to $\ell$.</p>





```input1|2,3,6,7,10,11,14,15,18,19
9
1 3 5
0
3 2 5
2 5 5
1 10 10
10
10 1 10
0 1 2 3 4 5 6 7 8 9
2 1 2
0 0
2 1 2
0 2
2 1 3
0 2
2 2 4
1 1
9 12 54
3 3 8 24 25 27 29 34 53
```




```output1
4
5
20
0
2
1
2
2
7
```



## Note

<p>In the first test case, the crow instantly teleports to position $3$ due to the scarecrow at position $0$. This scarecrow may then move to position $2$, causing the crow to continuously move from position $3$ to position $5$, completing the trip in $2$ seconds. Therefore, the output is $4$.</p><p>In the second test case, scarecrow $1$ and scarecrow $2$ can move to positions $0$ and $3$, respectively, in $2$ seconds, while scarecrow $3$ remains at position $5$. The crow teleports to position $2$ due to scarecrow $1$. Then, scarecrow $1$ moves to the right while scarecrow $2$ and scarecrow $3$ move to the left for $0.5$ seconds. This causes the crow to continuously move from position $2$ to position $2.5$ due to scarecrow $1$ moving right from position $0$. After this half second, the scarecrows will be at positions $0.5, 2.5, 4.5$. Scarecrow $2$, now at position $2.5$, causes the crow to instantly teleport to position $4.5$, and scarecrow $3$ at position $4.5$ causes it to instantly teleport to position $6.5$, which exceeds $\ell = 5$. Therefore, the crow finishes the trip in just $2.5$ seconds, and the output is $5$.</p><p>It can be shown that these are the minimum possible times for both test cases.</p>
