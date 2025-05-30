## Description

<div><p>One Saturday afternoon Egor was playing his favorite RPG game. While discovering new lands and territories, he came across the following sign:</p><center> <img class="tex-graphics" src="./29844/file/DHD23cO5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Egor is a passionate player, but he is an algorithmician as well. That's why he instantly spotted four common letters in two words on the sign above&nbsp;！ if we <span class="tex-font-style-it">permute</span> the letters "R", "E", "G", "O" from the first word, we can obtain the letters "O", "G", "R", "E". Egor got inspired by the sign and right away he came up with a problem about permutations.</p><p>You are given a permutation of length $n$. You have to split it into some non-empty subsequences so that each element of the permutation belongs to exactly one subsequence. Each subsequence must be <span class="tex-font-style-it">monotonic</span>&nbsp;！ that is, either increasing or decreasing.</p><p>Sequence is called to be a <span class="tex-font-style-it">subsequence</span> if it can be derived from permutation by deleting some (possibly none) elements without changing the order of the remaining elements.</p><p>The number of subsequences should be small enough&nbsp;！ let $f(n)$ be the minimum integer $k$ such that every permutation of length $n$ can be partitioned into at most $k$ monotonic subsequences.</p><p>You need to split the permutation into at most $f(n)$ monotonic subsequences.</p></div><div class="input-specification"><p>The first line contains one integer $t$ ($1 \leq t \leq 10^5$) ！ the number of test cases.</p><p><span class="tex-font-style-bf">You can only use $t = 1$ in hacks.</span></p><p>Next, descriptions of $t$ test cases come, each of them in the following format.</p><p>The first line of a single test case contains one integer $n$ ($1 \leq n \leq 10^5$) ！ the length of the permutation. The second line contains $n$ distinct integers $a_i$ ($1 \leq a_i \leq n$) ！ the permutation itself.</p><p>The sum of the values of $n$ over all test cases doesn't exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print the answer in the following format:</p><p>In the first line print $k$ ($1 \leq k \leq f(n)$) ！ the number of the subsequences in the partition. In the next $k$ lines, print the descriptions of found subsequences. Each description should start with a number $l_i$ ($1 \leq l_i \leq n$) ！ the length of the corresponding subsequence, followed by $l_i$ integers ！ the values of this subsequence in the order in which they occur in the permutation.</p><p>Each subsequence you output must be either increasing or decreasing. </p><p>In case there are multiple possible answers, print any of them.</p></div>

## Input

<p>The first line contains one integer $t$ ($1 \leq t \leq 10^5$) ！ the number of test cases.</p><p><span class="tex-font-style-bf">You can only use $t = 1$ in hacks.</span></p><p>Next, descriptions of $t$ test cases come, each of them in the following format.</p><p>The first line of a single test case contains one integer $n$ ($1 \leq n \leq 10^5$) ！ the length of the permutation. The second line contains $n$ distinct integers $a_i$ ($1 \leq a_i \leq n$) ！ the permutation itself.</p><p>The sum of the values of $n$ over all test cases doesn't exceed $10^5$.</p>

## Output

<p>For each test case print the answer in the following format:</p><p>In the first line print $k$ ($1 \leq k \leq f(n)$) ！ the number of the subsequences in the partition. In the next $k$ lines, print the descriptions of found subsequences. Each description should start with a number $l_i$ ($1 \leq l_i \leq n$) ！ the length of the corresponding subsequence, followed by $l_i$ integers ！ the values of this subsequence in the order in which they occur in the permutation.</p><p>Each subsequence you output must be either increasing or decreasing. </p><p>In case there are multiple possible answers, print any of them.</p>

## Samples

```input1
3
4
4 3 1 2
6
4 5 6 1 3 2
10
1 2 3 4 5 6 7 8 9 10
```

```output1
2
3 4 3 1
1 2
3
2 4 1
2 5 6
2 3 2
1
10 1 2 3 4 5 6 7 8 9 10
```




## Note

<p>In the example, we can split:</p><ul> <li> $[4, 3, 1, 2]$ into $[4, 3, 1]$, $[2]$ </li><li> $[4, 5, 6, 1, 3, 2]$ into $[4, 1]$, $[5, 6]$ and $[3, 2]$ </li><li> $[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]$ into $[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]$ </li></ul><p>Surely, there are many more answers possible.</p>
