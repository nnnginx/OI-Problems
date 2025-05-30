## Description

<div><p>Attention: we lost all the test cases for this problem, so instead of solving the problem, we need you to generate test cases. We're going to give you the answer, and you need to print a test case that produces the given answer. The original problem is in the following paragraph.</p><p>People don't use cash as often as they used to. Having a credit card solves some of the hassles of cash, such as having to receive change when you can't form the exact amount of money needed to purchase an item. Typically cashiers will give you as few coins as possible in change, but they don't have to. For example, if your change is 30 cents, a cashier could give you a 5 cent piece and a 25 cent piece, or they could give you three 10 cent pieces, or ten 1 cent pieces, two 5 cent pieces, and one 10 cent piece. Altogether there are 18 different ways to make 30 cents using only 1 cent pieces, 5 cent pieces, 10 cent pieces, and 25 cent pieces. Two ways are considered different if they contain a different number of at least one type of coin. Given the denominations of the coins and an amount of change to be made, how many different ways are there to make change?</p><p>As we mentioned before, we lost all the test cases for this problem, so we're actually going to give you the number of ways, and want you to produce a test case for which the number of ways is the given number. There could be many ways to achieve this (we guarantee there's always at least one), so you can print any, as long as it meets the constraints described below.</p></div><div class="input-specification"><p>Input will consist of a single integer <span class="tex-span"><i>A</i></span> <span class="tex-span">(1 ≤ <i>A</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the desired number of ways.</p></div><div class="output-specification"><p>In the first line print integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>M</i> ≤ 10)</span>, the amount of change to be made, and the number of denominations, respectively.</p><p>Then print <span class="tex-span"><i>M</i></span> integers <span class="tex-span"><i>D</i><sub class="lower-index">1</sub>, <i>D</i><sub class="lower-index">2</sub>, ..., <i>D</i><sub class="lower-index"><i>M</i></sub></span> <span class="tex-span">(1 ≤ <i>D</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>, the denominations of the coins. All denominations must be distinct: for any <span class="tex-span"><i>i</i> ≠ <i>j</i></span> we must have <span class="tex-span"><i>D</i><sub class="lower-index"><i>i</i></sub> ≠ <i>D</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>If there are multiple tests, print any of them. You can print denominations in atbitrary order.</p></div>

## Input

<p>Input will consist of a single integer <span class="tex-span"><i>A</i></span> <span class="tex-span">(1 ≤ <i>A</i> ≤ 10<sup class="upper-index">5</sup>)</span>, the desired number of ways.</p>

## Output

<p>In the first line print integers <span class="tex-span"><i>N</i></span> and <span class="tex-span"><i>M</i></span> <span class="tex-span">(1 ≤ <i>N</i> ≤ 10<sup class="upper-index">6</sup>, 1 ≤ <i>M</i> ≤ 10)</span>, the amount of change to be made, and the number of denominations, respectively.</p><p>Then print <span class="tex-span"><i>M</i></span> integers <span class="tex-span"><i>D</i><sub class="lower-index">1</sub>, <i>D</i><sub class="lower-index">2</sub>, ..., <i>D</i><sub class="lower-index"><i>M</i></sub></span> <span class="tex-span">(1 ≤ <i>D</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup>)</span>, the denominations of the coins. All denominations must be distinct: for any <span class="tex-span"><i>i</i> ≠ <i>j</i></span> we must have <span class="tex-span"><i>D</i><sub class="lower-index"><i>i</i></sub> ≠ <i>D</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>If there are multiple tests, print any of them. You can print denominations in atbitrary order.</p>

## Samples

```input1
18

```

```output1
30 4
1 5 10 25

```






```input2
3

```

```output2
20 2
5 2

```






```input3
314

```

```output3
183 4
6 5 2 139

```



