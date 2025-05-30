## Description

<div><p>SmallR is a biologist. Her latest research finding is how to change the sex of dogs. In other words, she can change female dogs into male dogs and vice versa.</p><p>She is going to demonstrate this technique. Now SmallR has <span class="tex-span"><i>n</i></span> dogs, the costs of each dog's change may be different. The dogs are numbered from 1 to <span class="tex-span"><i>n</i></span>. The cost of change for dog <span class="tex-span"><i>i</i></span> is <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> RMB. By the way, this technique needs a kind of medicine which can be valid for only one day. So the experiment should be taken in one day and each dog can be changed at most once.</p><p>This experiment has aroused extensive attention from all sectors of society. There are <span class="tex-span"><i>m</i></span> rich folks which are suspicious of this experiment. They all want to bet with SmallR forcibly. If SmallR succeeds, the <span class="tex-span"><i>i</i></span>-th rich folk will pay SmallR <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> RMB. But it's strange that they have a special method to determine whether SmallR succeeds. For <span class="tex-span"><i>i</i></span>-th rich folk, in advance, he will appoint certain <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> dogs and certain one gender. He will think SmallR succeeds if and only if on some day the <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> appointed dogs are all of the appointed gender. Otherwise, he will think SmallR fails.</p><p>If SmallR can't satisfy some folk that isn't her friend, she need not pay him, but if someone she can't satisfy is her good friend, she must pay <span class="tex-span"><i>g</i></span> RMB to him as apologies for her fail.</p><p>Then, SmallR hope to acquire money as much as possible by this experiment. Please figure out the maximum money SmallR can acquire. By the way, it is possible that she can't obtain any money, even will lose money. Then, please give out the minimum money she should lose.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>g</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 0 ≤ <i>m</i> ≤ 2000, 0 ≤ <i>g</i> ≤ 10<sup class="upper-index">4</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, each is 0 or 1, the sex of each dog, 0 represent the female and 1 represent the male. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes a rich folk. On the <span class="tex-span"><i>i</i></span>-th line the first number is the appointed sex of <span class="tex-span"><i>i</i></span>-th folk (0 or 1), the next two integers are <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>, next <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct integers are the indexes of appointed dogs (each index is between 1 and <span class="tex-span"><i>n</i></span>). The last number of this line represents whether <span class="tex-span"><i>i</i></span>-th folk is SmallR's good friend (0 — no or 1 — yes).</p></div><div class="output-specification"><p>Print a single integer, the maximum money SmallR can gain. Note that the integer is negative if SmallR will lose money. </p></div>


## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span>, <span class="tex-span"><i>g</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">4</sup>, 0 ≤ <i>m</i> ≤ 2000, 0 ≤ <i>g</i> ≤ 10<sup class="upper-index">4</sup>)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers, each is 0 or 1, the sex of each dog, 0 represent the female and 1 represent the male. The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(0 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>)</span>.</p><p>Each of the next <span class="tex-span"><i>m</i></span> lines describes a rich folk. On the <span class="tex-span"><i>i</i></span>-th line the first number is the appointed sex of <span class="tex-span"><i>i</i></span>-th folk (0 or 1), the next two integers are <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup>, 1 ≤ <i>k</i><sub class="lower-index"><i>i</i></sub> ≤ 10)</span>, next <span class="tex-span"><i>k</i><sub class="lower-index"><i>i</i></sub></span> distinct integers are the indexes of appointed dogs (each index is between 1 and <span class="tex-span"><i>n</i></span>). The last number of this line represents whether <span class="tex-span"><i>i</i></span>-th folk is SmallR's good friend (0 — no or 1 — yes).</p>


## Output

<p>Print a single integer, the maximum money SmallR can gain. Note that the integer is negative if SmallR will lose money. </p>


## Samples

```input1
5 5 9
0 1 1 1 0
1 8 6 2 3
0 7 3 3 2 1 1
1 8 1 5 1
1 0 3 2 1 4 1
0 8 3 4 2 1 0
1 7 2 4 1 1

```

```output1
2

```






```input2
5 5 8
1 0 1 1 1
6 5 4 2 8
0 6 3 2 3 4 0
0 8 3 3 2 4 0
0 0 3 3 4 1 1
0 10 3 4 3 1 1
0 4 3 3 4 1 1

```

```output2
16

```



