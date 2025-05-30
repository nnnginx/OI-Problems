## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>Ayush devised yet another scheme to set the password of his lock. The lock has $n$ slots where each slot can hold any non-negative integer. The password $P$ is a sequence of $n$ integers, $i$-th element of which goes into the $i$-th slot of the lock.</p><p>To set the password, Ayush comes up with an array $A$ of $n$ integers each in the range $[0, 2^{63}-1]$. He then sets the $i$-th element of $P$ as the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#OR">bitwise OR</a> of all integers in the array except $A_i$.</p><p>You need to guess the password. To make a query, you can choose a non-empty subset of indices of the array and ask the <span class="tex-font-style-bf">bitwise OR</span> all elements of the array with index in this subset. <span class="tex-font-style-bf">You can ask no more than 13 queries</span>.</p></div><div class="input-specification"><p>The first line of input contains one integer $n$ $(2 \le n \le 1000)$&nbsp;！ the number of slots in the lock.</p></div><div><h2>Interaction</h2><p>To ask a query print a single line: </p><ul> <li> In the beginning print "<span class="tex-font-style-tt">? c</span> " (without quotes) where $c$ $(1 \leq c \leq n)$ denotes the size of the subset of indices being queried, followed by $c$ <span class="tex-font-style-bf">distinct</span> space-separated integers in the range $[1, n]$. </li></ul><p>For each query, you will receive an integer $x$&nbsp;！ the bitwise OR of values in the array among all the indices queried. If the subset of indices queried is invalid or you exceeded the number of queries then you will get $x = -1$. In this case, you should terminate the program immediately.</p><p>When you have guessed the password, print a single line "<span class="tex-font-style-tt">!</span> " (without quotes), followed by $n$ space-separated integers &nbsp;！ the password sequence.</p><p>Guessing the password does <span class="tex-font-style-bf">not</span> count towards the number of queries asked.</p><p><span class="tex-font-style-bf">The interactor is not adaptive.</span> The array $A$ does not change with queries.</p><p>After printing a query do not forget to output the end of the line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul><li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++;</li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java;</li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal;</li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python;</li><li> see the documentation for other languages.</li></ul><p><span class="tex-font-style-bf">Hacks</span></p><p>To hack the solution, use the following test format:</p><p>On the first line print a single integer $n$ $(2 \le n \le 1000)$&nbsp;！ the number of slots in the lock. The next line should contain $n$ space-separated integers in the range $[0, 2^{63} - 1]$&nbsp;！ the array $A$.</p></div>

## Input

<p>The first line of input contains one integer $n$ $(2 \le n \le 1000)$&nbsp;！ the number of slots in the lock.</p>

## Samples

```input1
3

1

2

4
```

```output1
? 1 1

? 1 2

? 1 3

! 6 5 3
```




## Note

<p>The array $A$ in the example is $\{{1, 2, 4\}}$. The first element of the password is bitwise OR of $A_2$ and $A_3$, the second element is bitwise OR of $A_1$ and $A_3$ and the third element is bitwise OR of $A_1$ and $A_2$. Hence the password sequence is $\{{6, 5, 3\}}$.</p>
