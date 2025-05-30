## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is on constraints. In this version constraints are higher. You can make hacks only if all versions of the problem are solved.</span></p><p>Koa the Koala is at the beach!</p><p>The beach consists (from left to right) of a shore, $n+1$ meters of sea and an island at $n+1$ meters from the shore.</p><p>She measured the depth of the sea at $1, 2, \dots, n$ meters from the shore and saved them in array $d$. $d_i$ denotes the depth of the sea at $i$ meters from the shore for $1 \le i \le n$.</p><p>Like any beach this one has tide, the intensity of the tide is measured by parameter $k$ and affects all depths <span class="tex-font-style-bf">from the beginning at time $t=0$</span> in the following way:</p><ul> <li> For a total of $k$ seconds, each second, tide <span class="tex-font-style-bf">increases</span> all depths by $1$.<p> </p></li><li> Then, for a total of $k$ seconds, each second, tide <span class="tex-font-style-bf">decreases</span> all depths by $1$.<p> </p></li><li> This process repeats again and again (ie. depths increase for $k$ seconds then decrease for $k$ seconds and so on ...).<p>Formally, let's define $0$-indexed array $p = [0, 1, 2, \ldots, k - 2, k - 1, k, k - 1, k - 2, \ldots, 2, 1]$ of length $2k$. At time $t$ ($0 \le t$) depth at $i$ meters from the shore equals $d_i + p[t \bmod 2k]$ ($t \bmod 2k$ denotes the remainder of the division of $t$ by $2k$). Note that the changes occur <span class="tex-font-style-bf">instantaneously</span> after each second, see the notes for better understanding. </p></li></ul><p>At time $t=0$ Koa is standing at the shore and wants to get to the island. Suppose that at some time $t$ ($0 \le t$) she is at $x$ ($0 \le x \le n$) meters from the shore:</p><ul> <li> In one second Koa can swim $1$ meter further from the shore ($x$ changes to $x+1$) or not swim at all ($x$ stays the same), in both cases $t$ changes to $t+1$.<p> </p></li><li> As Koa is a bad swimmer, the depth of the sea at the point where she is can't exceed $l$ at integer points of time (or she will drown). More formally, if Koa is at $x$ ($1 \le x \le n$) meters from the shore at the moment $t$ (for some integer $t\ge 0$), the depth of the sea at this point &nbsp;！ $d_x + p[t \bmod 2k]$ &nbsp;！ can't exceed $l$. In other words, $d_x + p[t \bmod 2k] \le l$ must hold always.<p> </p></li><li> Once Koa reaches the island at $n+1$ meters from the shore, she stops and can rest.<p>Note that <span class="tex-font-style-bf">while Koa swims tide doesn't have effect on her</span> (ie. she can't drown while swimming). Note that <span class="tex-font-style-bf">Koa can choose to stay on the shore for as long as she needs</span> and <span class="tex-font-style-bf">neither the shore or the island are affected by the tide</span> (they are solid ground and she won't drown there). </p></li></ul><p>Koa wants to know whether she can go from the shore to the island. Help her!</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) &nbsp;！ the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $k$ and $l$ ($1 \le n \le 3 \cdot 10^5; 1 \le k \le 10^9; 1 \le l \le 10^9$)&nbsp;！ the number of meters of sea Koa measured and parameters $k$ and $l$.</p><p>The second line of each test case contains $n$ integers $d_1, d_2, \ldots, d_n$ ($0 \le d_i \le 10^9$) &nbsp;！ the depths of each meter of sea Koa measured.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case:</p><p>Print <span class="tex-font-style-tt">Yes</span> if Koa can get from the shore to the island, and <span class="tex-font-style-tt">No</span> otherwise.</p><p>You may print each letter in any case (upper or lower).</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 10^4$) &nbsp;！ the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains three integers $n$, $k$ and $l$ ($1 \le n \le 3 \cdot 10^5; 1 \le k \le 10^9; 1 \le l \le 10^9$)&nbsp;！ the number of meters of sea Koa measured and parameters $k$ and $l$.</p><p>The second line of each test case contains $n$ integers $d_1, d_2, \ldots, d_n$ ($0 \le d_i \le 10^9$) &nbsp;！ the depths of each meter of sea Koa measured.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $3 \cdot 10^5$.</p>

## Output

<p>For each test case:</p><p>Print <span class="tex-font-style-tt">Yes</span> if Koa can get from the shore to the island, and <span class="tex-font-style-tt">No</span> otherwise.</p><p>You may print each letter in any case (upper or lower).</p>

## Samples

```input1
7
2 1 1
1 0
5 2 3
1 2 3 2 2
4 3 4
0 2 4 3
2 3 5
3 0
7 2 3
3 0 2 1 3 0 1
7 1 4
4 4 3 0 2 4 2
5 2 3
1 2 3 2 2
```

```output1
Yes
No
Yes
Yes
Yes
No
No
```




## Note

<p>In the following $s$ denotes the shore, $i$ denotes the island, $x$ denotes distance from Koa to the shore, the underline denotes the position of Koa, and values in the array below denote current depths, <span class="tex-font-style-bf">affected by tide</span>, at $1, 2, \dots, n$ meters from the shore.</p><p>In test case $1$ we have $n = 2, k = 1, l = 1, p = [ 0, 1 ]$.</p><p>Koa wants to go from shore (at $x = 0$) to the island (at $x = 3$). Let's describe a possible solution:</p><ul> <li> Initially at $t = 0$ the beach looks like this: $[\underline{s}, 1, 0, i]$. </li><li> At $t = 0$ if Koa would decide to swim to $x = 1$, beach would look like: $[s, \underline{2}, 1, i]$ at $t = 1$, since $2 &gt; 1$ she would drown. So Koa waits $1$ second instead and beach looks like $[\underline{s}, 2, 1, i]$ at $t = 1$. </li><li> At $t = 1$ Koa swims to $x = 1$, beach looks like $[s, \underline{1}, 0, i]$ at $t = 2$. Koa doesn't drown because $1 \le 1$. </li><li> At $t = 2$ Koa swims to $x = 2$, beach looks like $[s, 2, \underline{1}, i]$ at $t = 3$. Koa doesn't drown because $1 \le 1$. </li><li> At $t = 3$ Koa swims to $x = 3$, beach looks like $[s, 1, 0, \underline{i}]$ at $t = 4$. </li><li> At $t = 4$ Koa is at $x = 3$ and she made it! </li></ul><p>We can show that in test case $2$ Koa can't get to the island.</p>
