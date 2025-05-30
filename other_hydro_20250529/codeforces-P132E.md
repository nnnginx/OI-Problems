## Description

<div><p>Another feature of Shakespeare language is that the variables are named after characters of plays by Shakespeare, and all operations on them (value assignment, output etc.) look like a dialog with other characters. New values of variables are defined in a rather lengthy way, so a programmer should try to minimize their usage.</p><p>You have to print the given sequence of <span class="tex-span"><i>n</i></span> integers. To do this, you have <span class="tex-span"><i>m</i></span> variables and two types of operations on them:</p><ul> <li> <span class="tex-font-style-tt">variable=integer</span> </li><li> <span class="tex-font-style-tt">print(variable)</span> </li></ul><p>Any of the <span class="tex-span"><i>m</i></span> variables can be used as <span class="tex-font-style-tt">variable</span>. Variables are denoted by lowercase letters between "<span class="tex-font-style-tt">a</span>" and "<span class="tex-font-style-tt">z</span>", inclusive. Any integer number can be used as <span class="tex-font-style-tt">integer</span>.</p><p>Let's say that the penalty for using first type of operations equals to the number of set bits in the number <span class="tex-font-style-tt">integer</span>. There is no penalty on using second type of operations. Find and output the program which minimizes the penalty for printing the given sequence of numbers.</p></div><div class="input-specification"><p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 26</span>). The second line contains the sequence to be printed. Each element of the sequence is an integer between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. The sequence has to be printed in the given order (from left to right).</p></div><div class="output-specification"><p>Output the number of lines in the optimal program and the optimal penalty. Next, output the program itself, one command per line. If there are several programs with minimal penalty, output any of them (you have only to minimize the penalty).</p></div>


## Input

<p>The first line of input contains integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 250</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 26</span>). The second line contains the sequence to be printed. Each element of the sequence is an integer between <span class="tex-span">1</span> and <span class="tex-span">10<sup class="upper-index">9</sup></span>, inclusive. The sequence has to be printed in the given order (from left to right).</p>


## Output

<p>Output the number of lines in the optimal program and the optimal penalty. Next, output the program itself, one command per line. If there are several programs with minimal penalty, output any of them (you have only to minimize the penalty).</p>


## Samples

```input1
7 2
1 2 2 4 2 1 2

```

```output1
11 4
b=1
print(b)
a=2
print(a)
print(a)
b=4
print(b)
print(a)
b=1
print(b)
print(a)

```






```input2
6 3
1 2 3 1 2 3

```

```output2
9 4
c=1
print(c)
b=2
print(b)
a=3
print(a)
print(c)
print(b)
print(a)

```



