## Description

<div><p>Fedya has a string $S$, initially empty, and an array $W$, also initially empty.</p><p>There are $n$ queries to process, one at a time. Query $i$ consists of a lowercase English letter $c_i$ and a nonnegative integer $w_i$. First, $c_i$ must be appended to $S$, and $w_i$ must be appended to $W$. The answer to the query is the sum of <span class="tex-font-style-it">suspiciousnesses</span> for all subsegments of $W$ $[L, \ R]$, $(1 \leq L \leq R \leq i)$.</p><p>We define the <span class="tex-font-style-it">suspiciousness</span> of a subsegment as follows: if the substring of $S$ corresponding to this subsegment (that is, a string of consecutive characters from $L$-th to $R$-th, inclusive) matches the prefix of $S$ of the same length (that is, a substring corresponding to the subsegment $[1, \ R - L + 1]$), then its suspiciousness is equal to the minimum in the array $W$ on the $[L, \ R]$ subsegment. Otherwise, in case the substring does not match the corresponding prefix, the suspiciousness is $0$.</p><p>Help Fedya answer all the queries before the orderlies come for him!</p></div><div class="input-specification"><p>The first line contains an integer $n$ $(1 \leq n \leq 600\,000)$&nbsp;！ the number of queries.</p><p>The $i$-th of the following $n$ lines contains the query $i$: a lowercase letter of the Latin alphabet $c_i$ and an integer $w_i$ $(0 \leq w_i \leq 2^{30} - 1)$.</p><p>All queries are given in an encrypted form. Let $ans$ be the answer to the previous query (for the first query we set this value equal to $0$). Then, in order to get the real query, you need to do the following: perform a cyclic shift of $c_i$ in the alphabet forward by $ans$, and set $w_i$ equal to $w_i \oplus (ans \ \&amp; \ MASK)$, where $\oplus$ is the bitwise exclusive "or", $\&amp;$ is the bitwise "and", and $MASK = 2^{30} - 1$.</p></div><div class="output-specification"><p>Print $n$ lines, $i$-th line should contain a single integer ！ the answer to the $i$-th query.</p></div>

## Input

<p>The first line contains an integer $n$ $(1 \leq n \leq 600\,000)$&nbsp;！ the number of queries.</p><p>The $i$-th of the following $n$ lines contains the query $i$: a lowercase letter of the Latin alphabet $c_i$ and an integer $w_i$ $(0 \leq w_i \leq 2^{30} - 1)$.</p><p>All queries are given in an encrypted form. Let $ans$ be the answer to the previous query (for the first query we set this value equal to $0$). Then, in order to get the real query, you need to do the following: perform a cyclic shift of $c_i$ in the alphabet forward by $ans$, and set $w_i$ equal to $w_i \oplus (ans \ \&amp; \ MASK)$, where $\oplus$ is the bitwise exclusive "or", $\&amp;$ is the bitwise "and", and $MASK = 2^{30} - 1$.</p>

## Output

<p>Print $n$ lines, $i$-th line should contain a single integer ！ the answer to the $i$-th query.</p>

## Samples

```input1
7
a 1
a 0
y 3
y 5
v 4
u 6
r 8
```

```output1
1
2
4
5
7
9
12
```






```input2
4
a 2
y 2
z 0
y 2
```

```output2
2
2
2
2
```






```input3
5
a 7
u 5
t 3
s 10
s 11
```

```output3
7
9
11
12
13
```




## Note

<p>For convenience, we will call "suspicious" those subsegments for which the corresponding lines are prefixes of $S$, that is, those whose suspiciousness may not be zero.</p><p>As a result of decryption in the first example, after all requests, the string $S$ is equal to "abacaba", and all $w_i = 1$, that is, the suspiciousness of all suspicious sub-segments is simply equal to $1$. Let's see how the answer is obtained after each request:</p><p>1. $S$ = "a", the array $W$ has a single subsegment ！ $[1, \ 1]$, and the corresponding substring is "a", that is, the entire string $S$, thus it is a prefix of $S$, and the suspiciousness of the subsegment is $1$.</p><p>2. $S$ = "ab", suspicious subsegments: $[1, \ 1]$ and $[1, \ 2]$, total $2$.</p><p>3. $S$ = "aba", suspicious subsegments: $[1, \ 1]$, $[1, \ 2]$, $[1, \ 3]$ and $[3, \ 3]$, total $4$.</p><p>4. $S$ = "abac", suspicious subsegments: $[1, \ 1]$, $[1, \ 2]$, $[1, \ 3]$, $[1, \ 4]$ and $[3, \ 3]$, total $5$.</p><p>5. $S$ = "abaca", suspicious subsegments: $[1, \ 1]$, $[1, \ 2]$, $[1, \ 3]$, $[1, \ 4]$ , $[1, \ 5]$, $[3, \ 3]$ and $[5, \ 5]$, total $7$.</p><p>6. $S$ = "abacab", suspicious subsegments: $[1, \ 1]$, $[1, \ 2]$, $[1, \ 3]$, $[1, \ 4]$ , $[1, \ 5]$, $[1, \ 6]$, $[3, \ 3]$, $[5, \ 5]$ and $[5, \ 6]$, total $9$.</p><p>7. $S$ = "abacaba", suspicious subsegments: $[1, \ 1]$, $[1, \ 2]$, $[1, \ 3]$, $[1, \ 4]$ , $[1, \ 5]$, $[1, \ 6]$, $[1, \ 7]$, $[3, \ 3]$, $[5, \ 5]$, $[5, \ 6]$, $[5, \ 7]$ and $[7, \ 7]$, total $12$.</p><p>In the second example, after all requests $S$ = "aaba", $W = [2, 0, 2, 0]$.</p><p>1. $S$ = "a", suspicious subsegments: $[1, \ 1]$ (suspiciousness $2$), totaling $2$.</p><p>2. $S$ = "aa", suspicious subsegments: $[1, \ 1]$ ($2$), $[1, \ 2]$ ($0$), $[2, \ 2]$ ( $0$), totaling $2$.</p><p>3. $S$ = "aab", suspicious subsegments: $[1, \ 1]$ ($2$), $[1, \ 2]$ ($0$), $[1, \ 3]$ ( $0$), $[2, \ 2]$ ($0$), totaling $2$.</p><p>4. $S$ = "aaba", suspicious subsegments: $[1, \ 1]$ ($2$), $[1, \ 2]$ ($0$), $[1, \ 3]$ ( $0$), $[1, \ 4]$ ($0$), $[2, \ 2]$ ($0$), $[4, \ 4]$ ($0$), totaling $2$.</p><p>In the third example, from the condition after all requests $S$ = "abcde", $W = [7, 2, 10, 1, 7]$.</p><p>1. $S$ = "a", suspicious subsegments: $[1, \ 1]$ ($7$), totaling $7$.</p><p>2. $S$ = "ab", suspicious subsegments: $[1, \ 1]$ ($7$), $[1, \ 2]$ ($2$), totaling $9$.</p><p>3. $S$ = "abc", suspicious subsegments: $[1, \ 1]$ ($7$), $[1, \ 2]$ ($2$), $[1, \ 3]$ ( $2$), totaling $11$.</p><p>4. $S$ = "abcd", suspicious subsegments: $[1, \ 1]$ ($7$), $[1, \ 2]$ ($2$), $[1, \ 3]$ ( $2$), $[1, \ 4]$ ($1$), totaling $12$.</p><p>5. $S$ = "abcde", suspicious subsegments: $[1, \ 1]$ ($7$), $[1, \ 2]$ ($2$), $[1, \ 3]$ ( $2$), $[1, \ 4]$ ($1$), $[1, \ 5]$ ($1$), totaling $13$.</p>
