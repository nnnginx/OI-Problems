## Description

<div><p>Petya studies in a school and he adores Maths. His class has been studying arithmetic expressions. On the last class the teacher wrote three positive integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> on the blackboard. The task was to insert signs of operations '<span class="tex-font-style-tt">+</span>' and '<span class="tex-font-style-tt">*</span>', and probably brackets between the numbers so that the value of the resulting expression is as large as possible. Let's consider an example: assume that the teacher wrote numbers 1, 2 and 3 on the blackboard. Here are some ways of placing signs and brackets:</p><ul> <li> 1+2*3=7 </li><li> 1*(2+3)=5 </li><li> 1*2*3=6 </li><li> (1+2)*3=9 </li></ul><p>Note that you can insert operation signs only between <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, and between <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, that is, you cannot swap integers. For instance, in the given sample you cannot get expression (1+3)*2.</p><p>It's easy to see that the maximum value that you can obtain is 9.</p><p>Your task is: given <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> print the maximum value that you can get.</p></div><div class="input-specification"><p>The input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, each on a single line (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10</span>).</p></div><div class="output-specification"><p>Print the maximum value of the expression that you can obtain.</p></div>


## Input

<p>The input contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span>, each on a single line (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 10</span>).</p>


## Output

<p>Print the maximum value of the expression that you can obtain.</p>


## Samples

```input1
1
2
3

```

```output1
9

```






```input2
2
10
3

```

```output2
60

```



