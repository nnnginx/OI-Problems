## Description

<div><p>Your friend has recently learned about coprime numbers. A pair of numbers <span class="tex-span">{<i>a</i>, <i>b</i>}</span> is called <span class="tex-font-style-it">coprime</span> if the maximum number that divides both <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is equal to one. </p><p>Your friend often comes up with different statements. He has recently supposed that if the pair <span class="tex-span">(<i>a</i>, <i>b</i>)</span> is coprime and the pair <span class="tex-span">(<i>b</i>, <i>c</i>)</span> is coprime, then the pair <span class="tex-span">(<i>a</i>, <i>c</i>)</span> is coprime. </p><p>You want to find a counterexample for your friend's statement. Therefore, your task is to find three distinct numbers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span>, for which the statement is false, and the numbers meet the condition <span class="tex-span"><i>l</i> ≤ <i>a</i> &lt; <i>b</i> &lt; <i>c</i> ≤ <i>r</i></span>. </p><p>More specifically, you need to find three numbers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span>, such that <span class="tex-span"><i>l</i> ≤ <i>a</i> &lt; <i>b</i> &lt; <i>c</i> ≤ <i>r</i></span>, pairs <span class="tex-span">(<i>a</i>, <i>b</i>)</span> and <span class="tex-span">(<i>b</i>, <i>c</i>)</span> are coprime, and pair <span class="tex-span">(<i>a</i>, <i>c</i>)</span> is not coprime.</p></div><div class="input-specification"><p>The single line contains two positive space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span"><i>r</i> - <i>l</i> ≤ 50</span>).</p></div><div class="output-specification"><p>Print three positive space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>&nbsp;— three distinct numbers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> that form the counterexample. If there are several solutions, you are allowed to print any of them. The numbers must be printed in ascending order. </p><p>If the counterexample does not exist, print the single number -1.</p></div>


## Input

<p>The single line contains two positive space-separated integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">18</sup></span>; <span class="tex-span"><i>r</i> - <i>l</i> ≤ 50</span>).</p>


## Output

<p>Print three positive space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span>&nbsp;— three distinct numbers <span class="tex-span">(<i>a</i>, <i>b</i>, <i>c</i>)</span> that form the counterexample. If there are several solutions, you are allowed to print any of them. The numbers must be printed in ascending order. </p><p>If the counterexample does not exist, print the single number -1.</p>


## Samples

```input1
2 4

```

```output1
2 3 4

```






```input2
10 11

```

```output2
-1

```






```input3
900000000000000009 900000000000000029

```

```output3
900000000000000009 900000000000000010 900000000000000021

```




## Note

<p>In the first sample pair <span class="tex-span">(2, 4)</span> is not coprime and pairs <span class="tex-span">(2, 3)</span> and <span class="tex-span">(3, 4)</span> are. </p><p>In the second sample you cannot form a group of three distinct integers, so the answer is -1. </p><p>In the third sample it is easy to see that numbers <span class="tex-span">900000000000000009</span> and <span class="tex-span">900000000000000021</span> are divisible by three. </p>

