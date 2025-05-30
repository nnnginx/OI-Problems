## Description

<div><p>Little Petya very much likes gifts. Recently he has received a new laptop as a New Year gift from his mother. He immediately decided to give it to somebody else as what can be more pleasant than giving somebody gifts. And on this occasion he organized a New Year party at his place and invited <span class="tex-span"><i>n</i></span> his friends there.</p><p>If there's one thing Petya likes more that receiving gifts, that's watching others giving gifts to somebody else. Thus, he safely hid the laptop until the next New Year and made up his mind to watch his friends exchanging gifts while he does not participate in the process. He numbered all his friends with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Petya remembered that a friend number <span class="tex-span"><i>i</i></span> gave a gift to a friend number <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. He also remembered that each of his friends received exactly one gift.</p><p>Now Petya wants to know for each friend <span class="tex-span"><i>i</i></span> the number of a friend who has given him a gift.</p></div><div class="input-specification"><p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the quantity of friends Petya invited to the party. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the number of a friend who gave a gift to friend number <span class="tex-span"><i>i</i></span>. It is guaranteed that each friend received exactly one gift. It is possible that some friends do not share Petya's ideas of giving gifts to somebody else. Those friends gave the gifts to themselves.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number should equal the number of the friend who gave a gift to friend number <span class="tex-span"><i>i</i></span>.</p></div>


## Input

<p>The first line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the quantity of friends Petya invited to the party. The second line contains <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number is <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> — the number of a friend who gave a gift to friend number <span class="tex-span"><i>i</i></span>. It is guaranteed that each friend received exactly one gift. It is possible that some friends do not share Petya's ideas of giving gifts to somebody else. Those friends gave the gifts to themselves.</p>


## Output

<p>Print <span class="tex-span"><i>n</i></span> space-separated integers: the <span class="tex-span"><i>i</i></span>-th number should equal the number of the friend who gave a gift to friend number <span class="tex-span"><i>i</i></span>.</p>


## Samples

```input1
4
2 3 4 1

```

```output1
4 1 2 3

```






```input2
3
1 3 2

```

```output2
1 3 2

```






```input3
2
1 2

```

```output3
1 2

```



