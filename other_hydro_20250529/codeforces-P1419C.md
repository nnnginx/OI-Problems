## Description

<div><p>A new agent called Killjoy invented a virus COVID-2069 that infects accounts on Codeforces. Each account has a rating, described by <span class="tex-font-style-bf">an integer</span> (it can possibly be negative or very large).</p><p>Killjoy's account is already infected and has a rating equal to $x$. Its rating is constant. There are $n$ accounts except hers, numbered from $1$ to $n$. The $i$-th account's initial rating is $a_i$. Any infected account (initially the only infected account is Killjoy's) instantly infects any uninfected account if their ratings are equal. This can happen at the beginning (before any rating changes) and after each contest. If an account is infected, it can not be healed.</p><p>Contests are regularly held on Codeforces. In each contest, any of these $n$ accounts (including infected ones) can participate. Killjoy can't participate. After each contest ratings are changed this way: each participant's rating is changed by an integer, but the sum of all changes must be equal to zero. New ratings can be any integer.</p><p>Find out the minimal number of contests needed to infect all accounts. You can choose which accounts will participate in each contest and how the ratings will change.</p><p>It can be proven that all accounts can be infected in some finite number of contests.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases. The next $2t$ lines contain the descriptions of all test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($2 \le n \le 10^3$, $-4000 \le x \le 4000$)&nbsp;！ the number of accounts on Codeforces and the rating of Killjoy's account.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ $(-4000 \le a_i \le 4000)$&nbsp;！ the ratings of other accounts.</p></div><div class="output-specification"><p>For each test case output the minimal number of contests needed to infect all accounts.</p></div>

## Input

<p>The first line contains a single integer $t$ $(1 \le t \le 100)$&nbsp;！ the number of test cases. The next $2t$ lines contain the descriptions of all test cases.</p><p>The first line of each test case contains two integers $n$ and $x$ ($2 \le n \le 10^3$, $-4000 \le x \le 4000$)&nbsp;！ the number of accounts on Codeforces and the rating of Killjoy's account.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \dots, a_n$ $(-4000 \le a_i \le 4000)$&nbsp;！ the ratings of other accounts.</p>

## Output

<p>For each test case output the minimal number of contests needed to infect all accounts.</p>

## Samples

```input1
3
2 69
68 70
6 4
4 4 4 4 4 4
9 38
-21 83 50 -59 -77 15 -71 -78 20
```

```output1
1
0
2
```




## Note

<p>In the first test case it's possible to make all ratings equal to $69$. First account's rating will increase by $1$, and second account's rating will decrease by $1$, so the sum of all changes will be equal to zero.</p><p>In the second test case all accounts will be instantly infected, because all ratings (including Killjoy's account's rating) are equal to $4$.</p>
