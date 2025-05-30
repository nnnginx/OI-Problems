## Description

<div><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>There is an unknown integer $x$ ($1\le x\le n$). You want to find $x$.</p><p>At first, you have a set of integers $\{1, 2, \ldots, n\}$. You can perform the following operations no more than $10000$ times:</p><ul> <li> <span class="tex-font-style-tt">A</span> $a$: find how many numbers are multiples of $a$ in the current set. </li><li> <span class="tex-font-style-tt">B</span> $a$: find how many numbers are multiples of $a$ in this set, and then delete all multiples of $a$, but $x$ will never be deleted (even if it is a multiple of $a$). In this operation, $a$ must be greater than $1$. </li><li> <span class="tex-font-style-tt">C</span> $a$: it means that you know that $x=a$. This operation can be only performed once. </li></ul><p>Remember that in the operation of type <span class="tex-font-style-tt">B</span> $a&gt;1$ must hold.</p><p>Write a program, that will find the value of $x$.</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1\le n\le 10^5$). The remaining parts of the input will be given throughout the interaction process.</p></div><div><h2>Interaction</h2><p>In each round, your program needs to print a line containing one uppercase letter <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span> or <span class="tex-font-style-tt">C</span> and an integer $a$ ($1\le a\le n$ for operations <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">C</span>, $2\le a\le n$ for operation <span class="tex-font-style-tt">B</span>). This line desribes operation you make.</p><p>If your operation has type <span class="tex-font-style-tt">C</span> your program should terminate immediately.</p><p>Else your program should read one line containing a single integer, which is the answer to your operation.</p><p>After outputting each line, don't forget to flush the output. To do it use:</p><ul> <li> fflush(stdout) in C/C++; </li><li> System.out.flush() in Java; </li><li> sys.stdout.flush() in Python; </li><li> flush(output) in Pascal; </li><li> See the documentation for other languages. </li></ul><p>It is guaranteed, that the number $x$ is fixed and won't change during the interaction process.</p><p><span class="tex-font-style-bf">Hacks:</span></p><p>To make a hack, use such input format:</p><p>The only line should contain two integers $n$, $x$ ($1 \leq x \leq n \leq 10^5$).</p></div>

## Input

<p>The first line contains one integer $n$ ($1\le n\le 10^5$). The remaining parts of the input will be given throughout the interaction process.</p>

## Samples

```input1
10

2

4

0
```

```output1
B 4

A 2

A 8

C 4
```




## Note

<p>Note that to make the sample more clear, we added extra empty lines. You shouldn't print any extra empty lines during the interaction process.</p><p>In the first test $n=10$ and $x=4$.</p><p>Initially the set is: $\{1,2,3,4,5,6,7,8,9,10\}$.</p><p>In the first operation, you ask how many numbers are multiples of $4$ and delete them. The answer is $2$ because there are two numbers divisible by $4$: $\{4,8\}$. $8$ will be deleted but $4$ won't, because the number $x$ will never be deleted. Now the set is $\{1,2,3,4,5,6,7,9,10\}$.</p><p>In the second operation, you ask how many numbers are multiples of $2$. The answer is $4$ because there are four numbers divisible by $2$: $\{2,4,6,10\}$.</p><p>In the third operation, you ask how many numbers are multiples of $8$. The answer is $0$ because there isn't any number divisible by $8$ in the current set.</p><p>In the fourth operation, you know that $x=4$, which is the right answer.</p>
