## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>Note: the XOR-sum of an array $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$) is defined as $a_1 \oplus a_2 \oplus \ldots \oplus a_n$, where $\oplus$ denotes the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p>Little Dormi received an array of $n$ integers $a_1, a_2, \ldots, a_n$ for Christmas. However, while playing with it over the winter break, he accidentally dropped it into his XOR machine, and the array got lost.</p><p>The XOR machine is currently configured with a query size of $k$ (which you cannot change), and allows you to perform the following type of query: by giving the machine $k$ <span class="tex-font-style-bf">distinct</span> indices $x_1, x_2, \ldots, x_k$, it will output $a_{x_1} \oplus a_{x_2} \oplus \ldots \oplus a_{x_k}$.</p><p>As Little Dormi's older brother, you would like to help him recover the <span class="tex-font-style-bf">XOR-sum</span> of his array $a_1, a_2, \ldots, a_n$ by querying the XOR machine.</p><p>Little Dormi isn't very patient, so to be as fast as possible, you must query the XOR machine the <span class="tex-font-style-bf">minimum</span> number of times to find the XOR-sum of his array. Formally, let $d$ be the minimum number of queries needed to find the XOR-sum of any array of length $n$ with a query size of $k$. Your program will be accepted if you find the correct XOR-sum in at most $d$ queries.</p><p>Lastly, you also noticed that with certain configurations of the machine $k$ and values of $n$, it may not be possible to recover the XOR-sum of Little Dormi's lost array. If that is the case, you should report it as well.</p><p>The array $a_1, a_2, \ldots, a_n$ is fixed before you start querying the XOR machine and does not change with the queries.</p></div><div class="input-specification"><p>The only line of input contains the integers $n$ and $k$ ($1 \le n \le 500$, $1 \le k \le n$), the length of the lost array and the configured query size of the XOR machine.</p><p>Elements of the original array satisfy $1 \le a_i \le 10^9$.</p><p>It can be proven that that if it is possible to recover the XOR sum under the given constraints, it can be done in at most $500$ queries. That is, $d \le 500$.</p><p>After taking $n$ and $k$, begin interaction.</p></div><div class="output-specification"><p>If it is impossible to recover the XOR-sum of the array, output $-1$ <span class="tex-font-style-bf">immediately</span> after taking $n$ and $k$. Do not begin interaction.</p><p>Otherwise, when your program finds the XOR-sum of the lost array $a_1, a_2, \ldots, a_n$, report the answer in the following format: "<span class="tex-font-style-tt">! x</span>", where $x$ is the XOR sum of the array $a_1, a_2, \ldots, a_n$, and terminate your program normally immediately after flushing the output stream. </p><p>Note that answering does not count as a query.</p></div><div><h2>Interaction</h2><p>Each query is made in the format "<span class="tex-font-style-tt">? b</span>", where $b$ is an array of exactly $k$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $n$ denoting the indices of the elements in the lost array that you want to query the XOR sum of.</p><p>You will then receive an integer $x$, the XOR sum of the queried elements. It can be proven that $0 \le x \le 2 \cdot 10^9$ will always be true.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages.</li></ul><p><span class="tex-font-style-bf">If at any point you make an invalid query or try to make more than $500$ queries (which is the hard limit), the interaction will terminate immediately and give you a Wrong Answer verdict. Note that if you exceed $d$ queries, the interaction will continue normally unless you also exceed the $500$ query hard limit, though you will still receive a Wrong Answer verdict either way.</span></p><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack a solution, use the following format.</p><p>The first line contains the integers $n$ and $k$ ($1 \le n \le 500$, $1 \le k \le n$).</p><p>The second line contains the the array $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p></div>

## Input

<p>The only line of input contains the integers $n$ and $k$ ($1 \le n \le 500$, $1 \le k \le n$), the length of the lost array and the configured query size of the XOR machine.</p><p>Elements of the original array satisfy $1 \le a_i \le 10^9$.</p><p>It can be proven that that if it is possible to recover the XOR sum under the given constraints, it can be done in at most $500$ queries. That is, $d \le 500$.</p><p>After taking $n$ and $k$, begin interaction.</p>

## Output

<p>If it is impossible to recover the XOR-sum of the array, output $-1$ <span class="tex-font-style-bf">immediately</span> after taking $n$ and $k$. Do not begin interaction.</p><p>Otherwise, when your program finds the XOR-sum of the lost array $a_1, a_2, \ldots, a_n$, report the answer in the following format: "<span class="tex-font-style-tt">! x</span>", where $x$ is the XOR sum of the array $a_1, a_2, \ldots, a_n$, and terminate your program normally immediately after flushing the output stream. </p><p>Note that answering does not count as a query.</p>

## Samples

```input1
5 3

4

0

1
```

```output1
? 1 2 3

? 2 3 5

? 4 1 5

! 7
```






```input2
3 2
```

```output2
-1
```




## Note

<p>In the first example interaction, the array $a_1, a_2, \ldots, a_n$ is $2, 1, 7, 5, 6$ and its XOR-sum is $7$. </p><p>The first query made asks for indices $1,2,3$, so the response is $a_1 \oplus a_2 \oplus a_3 = 2 \oplus 1 \oplus 7 = 4$.</p><p>The second query made asks for indices $2,3,5$, so the response is $a_2 \oplus a_3 \oplus a_5 = 1 \oplus 7 \oplus 6 = 0$.</p><p>The third query made asks for indices $4,1,5$, so the response is $a_4 \oplus a_1 \oplus a_5 = 5 \oplus 2 \oplus 6 = 1$. Note that the indices may be output in any order.</p><p>Additionally, even though three queries were made in the example interaction, it is just meant to demonstrate the interaction format and <span class="tex-font-style-bf">does not</span> necessarily represent an optimal strategy.</p><p>In the second example interaction, there is no way to recover the XOR-sum of Little Dormi's array no matter what is queried, so the program immediately outputs $-1$ and exits.</p>
