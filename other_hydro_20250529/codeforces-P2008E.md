## Description

<div><p>Sakurako really loves <span class="tex-font-style-it">alternating strings</span>. She calls a string $s$ of lowercase Latin letters an <span class="tex-font-style-it">alternating string</span> if characters in the even positions are the same, if characters in the odd positions are the same, and the length of the string is <span class="tex-font-style-bf">even</span>.</p><p>For example, the strings '<span class="tex-font-style-tt">abab</span>' and '<span class="tex-font-style-tt">gg</span>' are <span class="tex-font-style-it">alternating</span>, while the strings '<span class="tex-font-style-tt">aba</span>' and '<span class="tex-font-style-tt">ggwp</span>' are not.</p><p>As a good friend, you decided to gift such a string, but you couldn't find one. Luckily, you can perform two types of operations on the string: </p><ol> <li> Choose an index $i$ and delete the $i$-th character from the string, which will reduce the length of the string by $1$. This type of operation can be performed <span class="tex-font-style-bf">no more than $1$ time</span>; </li><li> Choose an index $i$ and replace $s_i$ with any other letter. </li></ol><p>Since you are in a hurry, you need to determine the minimum number of operations required to make the string an <span class="tex-font-style-it">alternating</span> one.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single number $n$ ($1 \le n\le 2\cdot 10^5$) &nbsp;！ the length of the string.</p><p>The second line of each test case contains a string $s$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;！ the minimum number of operations required to turn the string $s$ into an <span class="tex-font-style-it">alternating</span> one.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$) &nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single number $n$ ($1 \le n\le 2\cdot 10^5$) &nbsp;！ the length of the string.</p><p>The second line of each test case contains a string $s$, consisting of lowercase Latin letters.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output a single integer&nbsp;！ the minimum number of operations required to turn the string $s$ into an <span class="tex-font-style-it">alternating</span> one.</p>





```input1|2,3,6,7,10,11,14,15,18,19
10
1
a
2
ca
3
aab
5
ababa
6
acdada
9
ejibmyyju
6
bbccbc
6
abacba
5
bcbca
5
dcbdb
```




```output1
1
0
1
1
2
6
2
3
1
1
```



## Note

<p>For the string <span class="tex-font-style-tt">ababa</span>, you can delete the first character to get <span class="tex-font-style-tt">baba</span>, which is an <span class="tex-font-style-it">alternating</span> string.</p><p>For the string <span class="tex-font-style-tt">acdada</span>, you can change the first two characters to get <span class="tex-font-style-tt">dadada</span>, which is an <span class="tex-font-style-it">alternating</span> string.</p>
