## Description

<div><p>New Year is coming in Tree World! In this world, as the name implies, there are <span class="tex-span"><i>n</i></span> cities connected by <span class="tex-span"><i>n</i> - 1</span> roads, and for any two distinct cities there always exists a path between them. The cities are numbered by integers from 1 to <span class="tex-span"><i>n</i></span>, and the roads are numbered by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i> - 1</span>. Let's define <span class="tex-span"><i>d</i>(<i>u</i>, <i>v</i>)</span> as total length of roads on the path between city <span class="tex-span"><i>u</i></span> and city <span class="tex-span"><i>v</i></span>.</p><p>As an annual event, people in Tree World repairs exactly one road per year. As a result, the length of one road decreases. It is already known that in the <span class="tex-span"><i>i</i></span>-th year, the length of the <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>-th road is going to become <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>, which is shorter than its length before. Assume that the current year is year <span class="tex-span">1</span>.</p><p>Three Santas are planning to give presents annually to all the children in Tree World. In order to do that, they need some preparation, so they are going to choose three distinct cities <span class="tex-span"><i>c</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>c</i><sub class="lower-index">3</sub></span> and make exactly one warehouse in each city. The <span class="tex-span"><i>k</i></span>-th (<span class="tex-span">1 ≤ <i>k</i> ≤ 3</span>) Santa will take charge of the warehouse in city <span class="tex-span"><i>c</i><sub class="lower-index"><i>k</i></sub></span>.</p><p>It is really boring for the three Santas to keep a warehouse alone. So, they decided to build an only-for-Santa network! The cost needed to build this network equals to <span class="tex-span"><i>d</i>(<i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>) + <i>d</i>(<i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub>) + <i>d</i>(<i>c</i><sub class="lower-index">3</sub>, <i>c</i><sub class="lower-index">1</sub>)</span> dollars. Santas are too busy to find the best place, so they decided to choose <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, <i>c</i><sub class="lower-index">3</sub></span> randomly uniformly over all triples of distinct numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Santas would like to know the expected value of the cost needed to build the network.</p><p>However, as mentioned, each year, the length of exactly one road decreases. So, the Santas want to calculate the expected after each length change. Help them to calculate the value.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree World.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads. The <span class="tex-span"><i>i</i></span>-th line of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>), denoting that the <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and the length of <span class="tex-span"><i>i</i></span>-th road is <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of road length changes.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the length changes. The <span class="tex-span"><i>j</i></span>-th line of them (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) contains two space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">3</sup></span>). It means that in the <span class="tex-span"><i>j</i></span>-th repair, the length of the <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>-th road becomes <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span>. It is guaranteed that <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> is smaller than the current length of the <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>-th road. The same road can be repaired several times.</p></div><div class="output-specification"><p>Output <span class="tex-span"><i>q</i></span> numbers. For each given change, print a line containing the expected cost needed to build the network in Tree World. The answer will be considered correct if its absolute and relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>


## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of cities in Tree World.</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines describe the roads. The <span class="tex-span"><i>i</i></span>-th line of them (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i> - 1</span>) contains three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">3</sup></span>), denoting that the <span class="tex-span"><i>i</i></span>-th road connects cities <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>, and the length of <span class="tex-span"><i>i</i></span>-th road is <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of road length changes.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the length changes. The <span class="tex-span"><i>j</i></span>-th line of them (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) contains two space-separated integers <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">3</sup></span>). It means that in the <span class="tex-span"><i>j</i></span>-th repair, the length of the <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>-th road becomes <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span>. It is guaranteed that <span class="tex-span"><i>w</i><sub class="lower-index"><i>j</i></sub></span> is smaller than the current length of the <span class="tex-span"><i>r</i><sub class="lower-index"><i>j</i></sub></span>-th road. The same road can be repaired several times.</p>


## Output

<p>Output <span class="tex-span"><i>q</i></span> numbers. For each given change, print a line containing the expected cost needed to build the network in Tree World. The answer will be considered correct if its absolute and relative error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>


## Samples

```input1
3
2 3 5
1 3 3
5
1 4
2 2
1 2
2 1
1 1

```

```output1
14.0000000000
12.0000000000
8.0000000000
6.0000000000
4.0000000000

```






```input2
6
1 5 3
5 3 2
6 1 7
1 4 4
5 2 3
5
1 2
2 1
3 5
4 1
5 2

```

```output2
19.6000000000
18.6000000000
16.6000000000
13.6000000000
12.6000000000

```




## Note

<p>Consider the first sample. There are 6 triples: <span class="tex-span">(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)</span>. Because <span class="tex-span"><i>n</i> = 3</span>, the cost needed to build the network is always <span class="tex-span"><i>d</i>(1, 2) + <i>d</i>(2, 3) + <i>d</i>(3, 1)</span> for all the triples. So, the expected cost equals to <span class="tex-span"><i>d</i>(1, 2) + <i>d</i>(2, 3) + <i>d</i>(3, 1)</span>.</p>

