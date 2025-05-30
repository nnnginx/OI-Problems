## Description

<div><p>Well, here is another math class task. In mathematics, GCD is the greatest common divisor, and it's an easy task to calculate the GCD between two positive integers.</p><p>A common divisor for two positive numbers is a number which both numbers are divisible by.</p><p>But your teacher wants to give you a harder task, in this task you have to find the greatest common divisor <span class="tex-span"><i>d</i></span> between two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> that is in a given range from <span class="tex-span"><i>low</i></span> to <span class="tex-span"><i>high</i></span> (inclusive), i.e. <span class="tex-span"><i>low</i> ≤ <i>d</i> ≤ <i>high</i></span>. It is possible that there is no common divisor in the given range.</p><p>You will be given the two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, then <span class="tex-span"><i>n</i></span> queries. Each query is a range from <span class="tex-span"><i>low</i></span> to <span class="tex-span"><i>high</i></span> and you have to answer each query.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, the two integers as described above (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains one integer <span class="tex-span"><i>n</i></span>, the number of queries (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). Then <span class="tex-span"><i>n</i></span> lines follow, each line contains one query consisting of two integers, <span class="tex-span"><i>low</i></span> and <span class="tex-span"><i>high</i></span> (<span class="tex-span">1 ≤ <i>low</i> ≤ <i>high</i> ≤ 10<sup class="upper-index">9</sup></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the result of the <span class="tex-span"><i>i</i></span>-th query in the input. If there is no common divisor in the given range for any query, you should print <span class="tex-font-style-tt">-1</span> as a result for this query.</p></div>


## Input

<p>The first line contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>, the two integers as described above (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">9</sup></span>). The second line contains one integer <span class="tex-span"><i>n</i></span>, the number of queries (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup></span>). Then <span class="tex-span"><i>n</i></span> lines follow, each line contains one query consisting of two integers, <span class="tex-span"><i>low</i></span> and <span class="tex-span"><i>high</i></span> (<span class="tex-span">1 ≤ <i>low</i> ≤ <i>high</i> ≤ 10<sup class="upper-index">9</sup></span>).</p>


## Output

<p>Print <span class="tex-span"><i>n</i></span> lines. The <span class="tex-span"><i>i</i></span>-th of them should contain the result of the <span class="tex-span"><i>i</i></span>-th query in the input. If there is no common divisor in the given range for any query, you should print <span class="tex-font-style-tt">-1</span> as a result for this query.</p>


## Samples

```input1
9 27
3
1 5
10 11
9 11

```

```output1
3
-1
9

```



