## Description

<div><p>Vasya has got two number: <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. However, Vasya finds number <span class="tex-span"><i>a</i></span> too short. So he decided to repeat the operation of lengthening number <span class="tex-span"><i>a</i></span> <span class="tex-span"><i>n</i></span> times.</p><p>One operation of lengthening a number means adding exactly one digit to the number (in the decimal notation) to the right provided that the resulting number is divisible by Vasya's number <span class="tex-span"><i>b</i></span>. If it is impossible to obtain the number which is divisible by <span class="tex-span"><i>b</i></span>, then the lengthening operation cannot be performed.</p><p>Your task is to help Vasya and print the number he can get after applying the lengthening operation to number <span class="tex-span"><i>a</i> <i>n</i></span> times.</p></div><div class="input-specification"><p>The first line contains three integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>n</i> (1 ≤ <i>a</i>, <i>b</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p></div><div class="output-specification"><p>In a single line print the integer without leading zeros, which Vasya can get when he applies the lengthening operations to number <span class="tex-span"><i>a</i> <i>n</i></span> times. If no such number exists, then print number -1. If there are multiple possible answers, print any of them.</p></div>


## Input

<p>The first line contains three integers: <span class="tex-span"><i>a</i>, <i>b</i>, <i>n</i> (1 ≤ <i>a</i>, <i>b</i>, <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>.</p>


## Output

<p>In a single line print the integer without leading zeros, which Vasya can get when he applies the lengthening operations to number <span class="tex-span"><i>a</i> <i>n</i></span> times. If no such number exists, then print number -1. If there are multiple possible answers, print any of them.</p>


## Samples

```input1
5 4 5

```

```output1
524848

```






```input2
12 11 1

```

```output2
121

```






```input3
260 150 10

```

```output3
-1

```



