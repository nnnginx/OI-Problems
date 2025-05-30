## Description

<div><p>There are $n$ water tanks in a row, $i$-th of them contains $a_i$ liters of water. The tanks are numbered from $1$ to $n$ from left to right.</p><p>You can perform the following operation: choose some subsegment $[l, r]$ ($1\le l \le r \le n$), and redistribute water in tanks $l, l+1, \dots, r$ evenly. In other words, replace each of $a_l, a_{l+1}, \dots, a_r$ by $\frac{a_l + a_{l+1} + \dots + a_r}{r-l+1}$. For example, if for volumes $[1, 3, 6, 7]$ you choose $l = 2, r = 3$, new volumes of water will be $[1, 4.5, 4.5, 7]$. <span class="tex-font-style-bf">You can perform this operation any number of times</span>.</p><p>What is the lexicographically smallest sequence of volumes of water that you can achieve?</p><p>As a reminder:</p><p>A sequence $a$ is lexicographically smaller than a sequence $b$ of the same length if and only if the following holds: in the first (leftmost) position where $a$ and $b$ differ, the sequence $a$ has a smaller element than the corresponding element in $b$.</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($1 \le n \le 10^6$)&nbsp;�� the number of water tanks.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;�� initial volumes of water in the water tanks, in liters.</p><p>Because of large input, reading input as doubles <span class="tex-font-style-bf">is not recommended</span>.</p></div><div class="output-specification"><p>Print the lexicographically smallest sequence you can get. In the $i$-th line print the final volume of water in the $i$-th tank.</p><p>Your answer is considered correct if the absolute or relative error of each $a_i$ does not exceed $10^{-9}$.</p><p>Formally, let your answer be $a_1, a_2, \dots, a_n$, and the jury's answer be $b_1, b_2, \dots, b_n$. Your answer is accepted if and only if $\frac{|a_i - b_i|}{\max{(1, |b_i|)}} \le 10^{-9}$ for each $i$.</p></div>

## Input

<p>The first line contains an integer $n$ ($1 \le n \le 10^6$)&nbsp;�� the number of water tanks.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^6$)&nbsp;�� initial volumes of water in the water tanks, in liters.</p><p>Because of large input, reading input as doubles <span class="tex-font-style-bf">is not recommended</span>.</p>

## Output

<p>Print the lexicographically smallest sequence you can get. In the $i$-th line print the final volume of water in the $i$-th tank.</p><p>Your answer is considered correct if the absolute or relative error of each $a_i$ does not exceed $10^{-9}$.</p><p>Formally, let your answer be $a_1, a_2, \dots, a_n$, and the jury's answer be $b_1, b_2, \dots, b_n$. Your answer is accepted if and only if $\frac{|a_i - b_i|}{\max{(1, |b_i|)}} \le 10^{-9}$ for each $i$.</p>

## Samples

```input1
4
7 5 5 7
```

```output1
5.666666667
5.666666667
5.666666667
7.000000000
```






```input2
5
7 8 8 10 12
```

```output2
7.000000000
8.000000000
8.000000000
10.000000000
12.000000000
```






```input3
10
3 9 5 5 1 7 5 3 8 7
```

```output3
3.000000000
5.000000000
5.000000000
5.000000000
5.000000000
5.000000000
5.000000000
5.000000000
7.500000000
7.500000000
```




## Note

<p>In the first sample, you can get the sequence by applying the operation for subsegment $[1, 3]$.</p><p>In the second sample, you can't get any lexicographically smaller sequence.</p>
