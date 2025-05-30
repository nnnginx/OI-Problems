## Description

<div><p>Thought it is already the XXI century, the Mass Media isn't very popular in Walrusland. The cities get news from messengers who can only travel along roads. The network of roads in Walrusland is built so that it is possible to get to any city from any other one in exactly one way, and the roads' lengths are equal.</p><p>The North Pole governor decided to carry out an information reform. Several cities were decided to be chosen and made regional centers. Maintaining a region center takes <span class="tex-span"><i>k</i></span> fishlars (which is a local currency) per year. It is assumed that a regional center always has information on the latest news.</p><p>For every city which is not a regional center, it was decided to appoint a regional center which will be responsible for keeping this city informed. In that case the maintenance costs will be equal to <span class="tex-span"><i>d</i><sub class="lower-index"><i>len</i></sub></span> fishlars per year, where <span class="tex-span"><i>len</i></span> is the distance from a city to the corresponding regional center, measured in the number of roads along which one needs to go.</p><p>Your task is to minimize the costs to carry out the reform.</p></div><div class="input-specification"><p>The first line contains two given numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 180, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, numbered starting with 1 (<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i> + 1</sub>, 0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the pairs of cities connected by a road.</p></div><div class="output-specification"><p>On the first line print the minimum number of fishlars needed for a year's maintenance. On the second line print <span class="tex-span"><i>n</i></span> numbers, where the <span class="tex-span"><i>i</i></span>-th number will represent the number of the regional center, appointed to the <span class="tex-span"><i>i</i></span>-th city. If the <span class="tex-span"><i>i</i></span>-th city is a regional center itself, then you should print number <span class="tex-span"><i>i</i></span>.</p><p>If there are several solutions to that problem, print any of them.</p></div>


## Input

<p>The first line contains two given numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 180, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, numbered starting with 1 (<span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>d</i><sub class="lower-index"><i>i</i> + 1</sub>, 0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>Next <span class="tex-span"><i>n</i> - 1</span> lines contain the pairs of cities connected by a road.</p>


## Output

<p>On the first line print the minimum number of fishlars needed for a year's maintenance. On the second line print <span class="tex-span"><i>n</i></span> numbers, where the <span class="tex-span"><i>i</i></span>-th number will represent the number of the regional center, appointed to the <span class="tex-span"><i>i</i></span>-th city. If the <span class="tex-span"><i>i</i></span>-th city is a regional center itself, then you should print number <span class="tex-span"><i>i</i></span>.</p><p>If there are several solutions to that problem, print any of them.</p>


## Samples

```input1
8 10
2 5 9 11 15 19 20
1 4
1 3
1 7
4 6
2 8
2 3
3 5

```

```output1
38
3 3 3 4 3 4 3 3
```



