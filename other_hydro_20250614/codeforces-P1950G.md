## Description

<div><p>Vladislav has a playlist consisting of $n$ songs, numbered from $1$ to $n$. Song $i$ has genre $g_i$ and writer $w_i$. He wants to make a playlist in such a way that every pair of adjacent songs either have the same writer or are from the same genre (or both). He calls such a playlist <span class="tex-font-style-it">exciting</span>. Both $g_i$ and $w_i$ are strings of length no more than $10^4$.</p><p>It might not always be possible to make an exciting playlist using all the songs, so the shuffling process occurs in two steps. First, some amount (possibly zero) of the songs are removed, and then the remaining songs in the playlist are rearranged to make it exciting.</p><p>Since Vladislav doesn't like when songs get removed from his playlist, he wants the making playlist to perform as few removals as possible. Help him find the minimum number of removals that need to be performed in order to be able to rearrange the rest of the songs to make the playlist exciting.</p></div><div class="input-specification"><p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 16$)&nbsp;！ the number of songs in the original playlist.</p><p>Then $n$ lines follow, the $i$-th of which contains two strings of lowercase letters $g_i$ and $w_i$ ($1 \leq |g_i|, |w_i| \leq 10^4$)&nbsp;！ the genre and the writer of the $i$-th song. Where $|g_i|$ and $|w_i|$ are lengths of the strings.</p><p>The sum of $2^n$ over all test cases does not exceed $2^{16}$.</p><p>The sum of $|g_i| + |w_i|$ over all test cases does not exceed $4 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of removals necessary so that the resulting playlist can be made exciting.</p></div>

## Input

<p>The first line of the input contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases. The description of test cases follows.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 16$)&nbsp;！ the number of songs in the original playlist.</p><p>Then $n$ lines follow, the $i$-th of which contains two strings of lowercase letters $g_i$ and $w_i$ ($1 \leq |g_i|, |w_i| \leq 10^4$)&nbsp;！ the genre and the writer of the $i$-th song. Where $|g_i|$ and $|w_i|$ are lengths of the strings.</p><p>The sum of $2^n$ over all test cases does not exceed $2^{16}$.</p><p>The sum of $|g_i| + |w_i|$ over all test cases does not exceed $4 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of removals necessary so that the resulting playlist can be made exciting.</p>





```input1|2,3,9,10,11,12,13,14,15,16
4
1
pop taylorswift
4
electronic themotans
electronic carlasdreams
pop themotans
pop irinarimes
7
rap eminem
rap drdre
rap kanyewest
pop taylorswift
indierock arcticmonkeys
indierock arcticmonkeys
punkrock theoffspring
4
a b
c d
e f
g h
```




```output1
0
0
4
3
```



## Note

<p>In the first test case, the playlist is already exciting.</p><p>In the second test case, if you have the songs in the order $4, 3, 1, 2$, it is exciting, so you don't need to remove any songs.</p><p>In the third test case, you can remove songs $4, 5, 6, 7$. Then the playlist with songs in the order $1, 2, 3$ is exciting.</p>
