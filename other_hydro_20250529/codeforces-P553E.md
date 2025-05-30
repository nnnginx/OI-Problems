## Description

<div><p>Kyoya Ootori wants to take the train to get to school. There are <span class="tex-span"><i>n</i></span> train stations and <span class="tex-span"><i>m</i></span> one-way train lines going between various stations. Kyoya is currently at train station <span class="tex-span">1</span>, and the school is at station <span class="tex-span"><i>n</i></span>. To take a train, he must pay for a ticket, and the train also takes a certain amount of time. However, the trains are not perfect and take random amounts of time to arrive at their destination. If Kyoya arrives at school strictly after <span class="tex-span"><i>t</i></span> time units, he will have to pay a fine of <span class="tex-span"><i>x</i></span>.</p><p>Each train line is described by a ticket price, and a probability distribution on the time the train takes. More formally, train line <span class="tex-span"><i>i</i></span> has ticket cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, and a probability distribution <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>k</i></sub></span> which denotes the probability that this train will take <span class="tex-span"><i>k</i></span> time units for all <span class="tex-span">1 ≤ <i>k</i> ≤ <i>t</i></span>. Amounts of time that each of the trains used by Kyouya takes are mutually independent random values (moreover, if Kyoya travels along the same train more than once, it is possible for the train to take different amounts of time and those amounts are also independent one from another). </p><p>Kyoya wants to get to school by spending the least amount of money in expectation (for the ticket price plus possible fine for being late). Of course, Kyoya has an optimal plan for how to get to school, and every time he arrives at a train station, he may recalculate his plan based on how much time he has remaining. What is the expected cost that Kyoya will pay to get to school if he moves optimally?</p></div><div class="input-specification"><p>The first line of input contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>t</i>, <i>x</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 20 000</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The next <span class="tex-span">2<i>m</i></span> lines contain the description of the trains. </p><p>The <span class="tex-span">2<i>i</i></span>-th line will have <span class="tex-span">3</span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>, representing a one way train from station <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with ticket cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). There will always be at least one path from any station to the school. </p><p>The <span class="tex-span">(2<i>i</i> + 1)</span>-th line will contain <span class="tex-span"><i>t</i></span> integers, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>p</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>p</i><sub class="lower-index"><i>i</i>, <i>t</i></sub></span> where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> / 100000</span> is the probability that this train will take <span class="tex-span"><i>k</i></span> units of time to traverse (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 100 000</span> for <span class="tex-span">1 ≤ <i>k</i> ≤ <i>t</i></span>, <img align="middle" class="tex-formula" src="./27456/file/NAiUBAo2.png" style="max-width: 100.0%;max-height: 100.0%;">). </p><p>It is guaranteed that there is no more than one train between each pair of platforms in each of the directions.</p></div><div class="output-specification"><p>Print a single real number that is equal to an optimal expected cost of getting to school. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>


## Input

<p>The first line of input contains four integers <span class="tex-span"><i>n</i>, <i>m</i>, <i>t</i>, <i>x</i></span> (<span class="tex-span">2  ≤  <i>n</i>  ≤ 50</span>, <span class="tex-span">1 ≤ <i>m</i> ≤ 100</span>, <span class="tex-span">1 ≤ <i>t</i> ≤ 20 000</span>, <span class="tex-span">0 ≤ <i>x</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The next <span class="tex-span">2<i>m</i></span> lines contain the description of the trains. </p><p>The <span class="tex-span">2<i>i</i></span>-th line will have <span class="tex-span">3</span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span>, representing a one way train from station <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> with ticket cost <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>). There will always be at least one path from any station to the school. </p><p>The <span class="tex-span">(2<i>i</i> + 1)</span>-th line will contain <span class="tex-span"><i>t</i></span> integers, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, 1</sub>, <i>p</i><sub class="lower-index"><i>i</i>, 2</sub>, ..., <i>p</i><sub class="lower-index"><i>i</i>, <i>t</i></sub></span> where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> / 100000</span> is the probability that this train will take <span class="tex-span"><i>k</i></span> units of time to traverse (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i>, <i>k</i></sub> ≤ 100 000</span> for <span class="tex-span">1 ≤ <i>k</i> ≤ <i>t</i></span>, <img align="middle" class="tex-formula" src="./27456/file/NAiUBAo2.png" style="max-width: 100.0%;max-height: 100.0%;">). </p><p>It is guaranteed that there is no more than one train between each pair of platforms in each of the directions.</p>


## Output

<p>Print a single real number that is equal to an optimal expected cost of getting to school. The answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>


## Samples

```input1
4 4 5 1
1 2 0
50000 0 50000 0 0
2 3 0
10000 0 0 0 90000
3 4 0
100000 0 0 0 0
2 4 0
0 0 0 50000 50000

```

```output1
0.7000000000

```






```input2
4 4 5 1
1 2 100
50000 0 50000 0 0
2 3 100
10000 0 0 0 90000
3 4 100
100000 0 0 0 0
2 4 100
0 0 0 50000 50000

```

```output2
200.7500000000

```




## Note

<p>The optimal strategy in the first case is as follows:</p><p>First, travel along first train line. With probability <span class="tex-span">1 / 2</span> Kyoya will take <span class="tex-span">1</span> time unit. Otherwise, Kyoya will take <span class="tex-span">3</span> time units.</p><p>If the train takes <span class="tex-span">1</span> time unit, travel along the 4th train line. Kyoya will make it to school in time with probability <span class="tex-span">1 / 2</span>. Otherwise, if the train takes 3 time units, travel along the 2nd train line. Kyoya will make it to school in time with probability <span class="tex-span">1 / 10</span>.</p><p>Since the cost of all train lines are zero, we can just look at the probability that Kyoya will incur the penalty. The probability that Kyoya will have to pay the penalty is <span class="tex-span">1 / 2 × 1 / 2 + 1 / 2 × 9 / 10 = 7 / 10</span>. We can show that no other strategy is strictly better.</p><p>The optimal strategy in the second case is to travel along <span class="tex-span">1 → 2 → 4</span> no matter what. Kyoya will incur the penalty with probability <span class="tex-span">3 / 4</span>, and the cost of the trains is <span class="tex-span">200</span>, thus the expected cost is <span class="tex-span">200.75</span>.</p>

