## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and hard versions is the constraints on the number of queries.</span></p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Ridbit has a hidden array $a$ of $n$ integers which he wants Ashish to guess. Note that $n$ is a <span class="tex-font-style-bf">power of two</span>. Ashish is allowed to ask three different types of queries. They are of the form </p><ul> <li> <span class="tex-font-style-tt">AND</span> $i$ $j$: ask for the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of elements $a_i$ and $a_j$ $(1 \leq i, j \le n$, $i \neq j)$ </li><li> <span class="tex-font-style-tt">OR</span> $i$ $j$: ask for the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of elements $a_i$ and $a_j$ $(1 \leq i, j \le n$, $i \neq j)$ </li><li> <span class="tex-font-style-tt">XOR</span> $i$ $j$: ask for the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR</a> of elements $a_i$ and $a_j$ $(1 \leq i, j \le n$, $i \neq j)$ </li></ul><p>Can you help Ashish guess the elements of the array?</p><p><span class="tex-font-style-bf">In this version, each element takes a value in the range $[0, n-1]$ (inclusive) and Ashish can ask no more than $n+2$ queries.</span></p></div><div class="input-specification"><p>The first line of input contains one integer $n$ $(4 \le n \le 2^{16})$&nbsp;！ the length of the array. It is guaranteed that $n$ is a <span class="tex-font-style-bf">power of two</span>.</p></div><div><h2>Interaction</h2><p>To ask a query print a single line containing one of the following (without quotes) </p><ul> <li> "<span class="tex-font-style-tt">AND i j</span>" </li><li> "<span class="tex-font-style-tt">OR i j</span>" </li><li> "<span class="tex-font-style-tt">XOR i j</span>" </li></ul> where $i$ and $j$ $(1 \leq i, j \le n$, $i \neq j)$ denote the indices being queried.<p>For each query, you will receive an integer $x$ whose value depends on the type of query. If the indices queried are invalid or you exceed the number of queries however, you will get $x = -1$. In this case, you should terminate the program immediately.</p><p>When you have guessed the elements of the array, print a single line "<span class="tex-font-style-tt">!</span> " (without quotes), followed by $n$ space-separated integers &nbsp;！ the elements of the array.</p><p>Guessing the array does <span class="tex-font-style-bf">not</span> count towards the number of queries asked.</p><p><span class="tex-font-style-bf">The interactor is not adaptive.</span> The array $a$ does not change with queries.</p><p>After printing a query do not forget to output the end of the line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution, use the following test format:</p><p>On the first line print a single integer $n$ $(4 \le n \le 2^{16})$&nbsp;！ the length of the array. It <span class="tex-font-style-bf">must</span> be a power of 2. The next line should contain $n$ space-separated integers in the range $[0, n-1]$&nbsp;！ the array $a$.</p></div>

## Input

<p>The first line of input contains one integer $n$ $(4 \le n \le 2^{16})$&nbsp;！ the length of the array. It is guaranteed that $n$ is a <span class="tex-font-style-bf">power of two</span>.</p>

## Samples

```input1
4

0

2

3
```

```output1
OR 1 2

OR 2 3

XOR 2 4

! 0 0 2 3
```




## Note

<p>The array $a$ in the example is $[0, 0, 2, 3]$.</p>
