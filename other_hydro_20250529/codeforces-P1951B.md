## Description

<div><div class="epigraph"><div class="epigraph-text"><a href="https://youtu.be/SNCx4n2m5_o"><span class="tex-font-style-it">The HU - Shireg Shireg</span></a></div><div class="epigraph-source">ඞ</div></div><p>There are $n$ cows participating in a coding tournament. Cow $i$ has a Cowdeforces rating of $a_i$ (all distinct), and is initially in position $i$. The tournament consists of $n-1$ matches as follows: </p><ul> <li> The first match is between the cow in position $1$ and the cow in position $2$. </li><li> Subsequently, each match $i$ is between the cow in position $i+1$ and the winner of match $i-1$. </li><li> In each match, the cow with the higher Cowdeforces rating wins and proceeds to the next match. </li></ul><p>You are the owner of cow $k$. For you, winning the tournament is not important; rather, you want your cow to win in as many matches as possible. As an acquaintance of the tournament organizers, you can ask them to swap the position of your cow with another cow <span class="tex-font-style-bf">only once</span>, or you can choose to do nothing.</p><p>Find the maximum number of wins your cow can achieve.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^5, 1 \le k \le n$)&nbsp;— the number of cows and your cow's index.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the Cowdeforces rating of the cows. It is guaranteed that $a_i$'s are pairwise different.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print one integer: the maximum number of wins cow $k$ can achieve if you choose to swap (or do nothing) optimally.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains an integer $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases. The description of the test cases follows.</p><p>The first line of each test case contains two integers $n$ and $k$ ($2 \le n \le 10^5, 1 \le k \le n$)&nbsp;— the number of cows and your cow's index.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;— the Cowdeforces rating of the cows. It is guaranteed that $a_i$'s are pairwise different.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print one integer: the maximum number of wins cow $k$ can achieve if you choose to swap (or do nothing) optimally.</p>





```input1|2,3,6,7
3
6 1
12 10 14 11 8 3
6 5
7 2 727 10 12 13
2 2
1000000000 1
```




```output1
1
2
0
```



## Note

<p>In the first test case, it is optimal to do nothing. Let $a'$ be the Cowdeforces rating of the cows in the original order (with your cow's rating bolded), then </p><ul> <li> Initially, $a' = [\mathbf{12}, 10, 14, 11, 8, 3]$. </li><li> Your cow plays against the cow with Cowdeforces rating $10$ and wins. $a' = [\mathbf{12}, 14, 11, 8, 3]$. </li><li> Your cow plays against the cow with Cowdeforces rating $14$ and loses. </li></ul> In total, your cow wins $1$ match.<p>In the second test case, it is optimal to swap your cow to position $3$. Then, let $a'$ be the Cowdeforces rating of the cows in the order after the swap. </p><ul> <li> Initially, $a' = [7, 2, \mathbf{12}, 10, 727, 13]$. </li><li> The cow with Cowdeforces rating $7$ plays against the cow with Cowdeforces rating $2$ and wins. $a' = [7, \mathbf{12}, 10, 727, 13]$. </li><li> The cow with Cowdeforces rating $7$ plays against your cow, and your cow wins. $a' = [\mathbf{12}, 10, 727, 13]$. </li><li> Your cow plays against the cow with Cowdeforces rating $10$ and wins. $a' = [\mathbf{12}, 727, 13]$. </li><li> Your cow plays against the cow with Cowdeforces rating $727$ and loses. </li></ul> In total, your cow wins $2$ matches.
