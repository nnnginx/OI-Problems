## Description

<div><p>After completing the first quest, Akito left the starting cave. After a while, he stumbled upon a goblin village.</p><p>Since Akito had nowhere to live, he wanted to find out the price of housing. It is well known that goblins write numbers as a string of characters '-' and '_', and the value represented by the string $s$ is the number of distinct subsequences$^{\text{∗}}$ of the string $s$ that are equal to the string "<span class="tex-font-style-tt">-_-</span>" (this is very similar to goblin faces).</p><p>For example, the string $s=$"<span class="tex-font-style-tt">-_--_-</span>" represents the number $6$, as it has $6$ subsequences "<span class="tex-font-style-tt">-_-</span>":</p><ol> <li> $s_1+s_2+s_3$ </li><li> $s_1+s_2+s_4$ </li><li> $s_1+s_2+s_6$ </li><li> $s_1+s_5+s_6$ </li><li> $s_3+s_5+s_6$ </li><li> $s_4+s_5+s_6$ </li></ol><p>Initially, the goblins wrote a random string-number $s$ in response to Akito's question, but then they realized that they wanted to take as much gold as possible from the traveler. To do this, they ask you to rearrange the characters in the string $s$ so that the value of the number represented by the string $s$ is maximized.</p><div class="statement-footnote"><p>$^{\text{∗}}$A subsequence of a string $a$ is a string $b$ that can be obtained by deleting several (possibly $0$) characters from $a$. Subsequences are considered different if they are obtained by deleting different sets of indices.</p></div></div><div class="input-specification"><p>The first line contains the number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>In the first line of each test case, there is one number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string written by the goblins.</p><p>In the second line of each test case, there is a string $s$ of length $n$, consisting only of characters '-' and '_'&nbsp;— the string written by the goblins.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, you need to output one number — the maximum number of subsequences equal to the string "-_-", if the characters in the string $s$ are optimally rearranged.</p></div>

## Input

<p>The first line contains the number $t$ ($1 \le t \le 10^4$)&nbsp;— the number of test cases.</p><p>In the first line of each test case, there is one number $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;— the length of the string written by the goblins.</p><p>In the second line of each test case, there is a string $s$ of length $n$, consisting only of characters '-' and '_'&nbsp;— the string written by the goblins.</p><p>It is guaranteed that the sum of $n$ across all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, you need to output one number — the maximum number of subsequences equal to the string "-_-", if the characters in the string $s$ are optimally rearranged.</p>





```input1|2,3,6,7,10,11,14,15
8
3
--_
5
__-__
9
--__-_---
4
_--_
10
_-_-_-_-_-
7
_------
1
-
2
_-
```




```output1
1
0
27
2
30
9
0
0
```



## Note

<p>In the first test case, it is beneficial to rearrange the characters to form the string "-_-". This is the only string of three characters that has at least one subsequence "-_-".</p><p>In the second test case, there is only one character "-", and at least two are needed for the subsequence "-_-". This means that for any rearrangement of characters, the answer will be $0$.</p><p>In the seventh and eighth test cases, the length of the string $n &lt; 3$, which means that subsequences of length $3$ do not exist.</p>
