## Description

<div><p>Arkady has a playlist that initially consists of $n$ songs, numerated from $1$ to $n$ in the order they appear in the playlist. Arkady starts listening to the songs in the playlist one by one, starting from song $1$. The playlist is cycled, i.&nbsp;e. after listening to the last song, Arkady will continue listening from the beginning.</p><p>Each song has a genre $a_i$, which is a positive integer. Let Arkady finish listening to a song with genre $y$, and the genre of the next-to-last listened song be $x$. If $\operatorname{gcd}(x, y) = 1$, he deletes the last listened song (with genre $y$) from the playlist. After that he continues listening normally, skipping the deleted songs, and <span class="tex-font-style-bf">forgetting</span> about songs he listened to before. In other words, after he deletes a song, he can't delete the next song immediately.</p><p>Here $\operatorname{gcd}(x, y)$ denotes the <a href="https://en.wikipedia.org/wiki/Greatest_common_divisor">greatest common divisor (GCD)</a> of integers $x$ and $y$.</p><p>For example, if the initial songs' genres were $[5, 9, 2, 10, 15]$, then the playlist is converted as follows: [<span class="tex-font-style-bf">5</span>, 9, 2, 10, 15] $\to$ [<span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">9</span>, 2, 10, 15] $\to$ [5, 2, 10, 15] (because $\operatorname{gcd}(5, 9) = 1$) $\to$ [5, <span class="tex-font-style-bf">2</span>, 10, 15] $\to$ [5, <span class="tex-font-style-bf">2</span>, <span class="tex-font-style-bf">10</span>, 15] $\to$ [5, 2, <span class="tex-font-style-bf">10</span>, <span class="tex-font-style-bf">15</span>] $\to$ [<span class="tex-font-style-bf">5</span>, 2, 10, <span class="tex-font-style-bf">15</span>] $\to$ [<span class="tex-font-style-bf">5</span>, <span class="tex-font-style-bf">2</span>, 10, 15] $\to$ [5, 10, 15] (because $\operatorname{gcd}(5, 2) = 1$) $\to$ [5, <span class="tex-font-style-bf">10</span>, 15] $\to$ [5, <span class="tex-font-style-bf">10</span>, <span class="tex-font-style-bf">15</span>] $\to$ ... The bold numbers represent the two last played songs. Note that after a song is deleted, Arkady forgets that he listened to that and the previous songs.</p><p>Given the initial playlist, please determine which songs are eventually deleted and the order these songs are deleted.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of songs.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the genres of the songs.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print a single line. First, print a single integer $k$&nbsp;！ the number of deleted songs. After that print $k$ distinct integers: deleted songs in the order of their deletion.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10\,000$). Description of the test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the number of songs.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$)&nbsp;！ the genres of the songs.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print a single line. First, print a single integer $k$&nbsp;！ the number of deleted songs. After that print $k$ distinct integers: deleted songs in the order of their deletion.</p>

## Samples

```input1
5
5
5 9 2 10 15
6
1 2 4 2 4 2
2
1 2
1
1
1
2
```

```output1
2 2 3 
2 2 1 
2 2 1 
1 1 
0
```




## Note

<p>Explanation of the first test case is given in the statement.</p><p>In the second test case, the playlist is converted as follows: [<span class="tex-font-style-bf">1</span>, 2, 4, 2, 4, 2] $\to$ [<span class="tex-font-style-bf">1</span>, <span class="tex-font-style-bf">2</span>, 4, 2, 4, 2] $\to$ [1, 4, 2, 4, 2] (because $\operatorname{gcd}(1, 2) = 1$) $\to$ [1, <span class="tex-font-style-bf">4</span>, 2, 4, 2] $\to$ [1, <span class="tex-font-style-bf">4</span>, <span class="tex-font-style-bf">2</span>, 4, 2] $\to$ [1, 4, <span class="tex-font-style-bf">2</span>, <span class="tex-font-style-bf">4</span>, 2] $\to$ [1, 4, 2, <span class="tex-font-style-bf">4</span>, <span class="tex-font-style-bf">2</span>] $\to$ [<span class="tex-font-style-bf">1</span>, 4, 2, 4, <span class="tex-font-style-bf">2</span>] $\to$ [4, 2, 4, 2] (because $\operatorname{gcd}(2, 1) = 1$) $\to$ [<span class="tex-font-style-bf">4</span>, 2, 4, 2] $\to$ ...</p><p>In the third test case, the playlist is converted as follows: [<span class="tex-font-style-bf">1</span>, 2] $\to$ [<span class="tex-font-style-bf">1</span>, <span class="tex-font-style-bf">2</span>] $\to$ [1] (because $\operatorname{gcd}(1, 2) = 1$) $\to$ [<span class="tex-font-style-bf">1</span>] $\to$ [<span class="tex-font-style-bf">1</span>] (Arkady listened to the same song twice in a row) $\to$ [] (because $\operatorname{gcd}(1, 1) = 1$).</p><p>The fourth test case is same as the third after deletion of the second song.</p><p>In the fifth test case, the same song is listened to over and over again, but since $\operatorname{gcd}(2, 2) \ne 1$, it is not deleted.</p>
