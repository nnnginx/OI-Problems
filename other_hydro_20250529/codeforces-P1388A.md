## Description

<div><p><span class="tex-font-style-it">Despite his bad reputation, Captain Flint is a friendly person (at least, friendly to animals). Now Captain Flint is searching worthy sailors to join his new crew (solely for peaceful purposes). A sailor is considered as worthy if he can solve Flint's task.</span></p><p>Recently, out of blue Captain Flint has been interested in math and even defined a new class of integers. Let's define a positive integer $x$ as <span class="tex-font-style-bf">nearly prime</span> if it can be represented as $p \cdot q$, where $1 &lt; p &lt; q$ and $p$ and $q$ are prime numbers. For example, integers $6$ and $10$ are nearly primes (since $2 \cdot 3 = 6$ and $2 \cdot 5 = 10$), but integers $1$, $3$, $4$, $16$, $17$ or $44$ are not.</p><p>Captain Flint guessed an integer $n$ and asked you: can you represent it as <span class="tex-font-style-it">the sum of $4$ <span class="tex-font-style-bf">different positive</span> integers</span> where <span class="tex-font-style-bf">at least $3$</span> of them should be <span class="tex-font-style-it">nearly prime</span>.</p><p>Uncle Bogdan easily solved the task and joined the crew. Can you do the same?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;！ one per line. The first and only line of each test case contains the single integer $n$ $(1 \le n \le 2 \cdot 10^5)$&nbsp;！ the number Flint guessed.</p></div><div class="output-specification"><p>For each test case print: </p><ul> <li> <span class="tex-font-style-tt">YES</span> and $4$ <span class="tex-font-style-bf">different</span> positive integers such that at least $3$ of them are nearly prime and their sum is equal to $n$ (if there are multiple answers print any of them); </li><li> <span class="tex-font-style-tt">NO</span> if there is no way to represent $n$ as <span class="tex-font-style-it">the sum of $4$ <span class="tex-font-style-bf">different positive</span> integers</span> where at least $3$ of them are nearly prime. </li></ul> You can print each character of <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in any case.</div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;！ the number of test cases.</p><p>Next $t$ lines contain test cases&nbsp;！ one per line. The first and only line of each test case contains the single integer $n$ $(1 \le n \le 2 \cdot 10^5)$&nbsp;！ the number Flint guessed.</p>

## Output

<p>For each test case print: </p><ul> <li> <span class="tex-font-style-tt">YES</span> and $4$ <span class="tex-font-style-bf">different</span> positive integers such that at least $3$ of them are nearly prime and their sum is equal to $n$ (if there are multiple answers print any of them); </li><li> <span class="tex-font-style-tt">NO</span> if there is no way to represent $n$ as <span class="tex-font-style-it">the sum of $4$ <span class="tex-font-style-bf">different positive</span> integers</span> where at least $3$ of them are nearly prime. </li></ul> You can print each character of <span class="tex-font-style-tt">YES</span> or <span class="tex-font-style-tt">NO</span> in any case.

## Samples

```input1
7
7
23
31
36
44
100
258
```

```output1
NO
NO
YES
14 10 6 1
YES
5 6 10 15
YES
6 7 10 21
YES
2 10 33 55
YES
10 21 221 6
```




## Note

<p>In the first and second test cases, it can be proven that there are no four different positive integers such that at least three of them are nearly prime.</p><p>In the third test case, $n=31=2 \cdot 7 + 2 \cdot 5 + 2 \cdot 3 + 1$: integers $14$, $10$, $6$ are nearly prime.</p><p>In the fourth test case, $n=36=5 + 2 \cdot 3 + 2 \cdot 5 + 3 \cdot 5$: integers $6$, $10$, $15$ are nearly prime.</p><p>In the fifth test case, $n=44=2 \cdot 3 + 7 + 2 \cdot 5 + 3 \cdot 7$: integers $6$, $10$, $21$ are nearly prime.</p><p>In the sixth test case, $n=100=2 + 2 \cdot 5 + 3 \cdot 11 + 5 \cdot 11$: integers $10$, $33$, $55$ are nearly prime.</p><p>In the seventh test case, $n=258=2 \cdot 5 + 3 \cdot 7 + 13 \cdot 17 + 2 \cdot 3$: integers $10$, $21$, $221$, $6$ are nearly prime.</p>
