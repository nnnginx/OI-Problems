## Description

<div><p>A country named Berland has <span class="tex-span"><i>n</i></span> cities. They are numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. City with index <span class="tex-span">1</span> is the capital of the country. Some pairs of cities have monodirectional roads built between them. However, not all of them are in good condition. For each road we know whether it needs repairing or not. If a road needs repairing, then it is forbidden to use it. However, the Berland government can repair the road so that it can be used.</p><p>Right now Berland is being threatened by the war with the neighbouring state. So the capital officials decided to send a military squad to each city. The squads can move only along the existing roads, as there's no time or money to build new roads. However, some roads will probably have to be repaired in order to get to some cities.</p><p>Of course the country needs much resources to defeat the enemy, so you want to be careful with what you're going to throw the forces on. That's why the Berland government wants to repair the minimum number of roads that is enough for the military troops to get to any city from the capital, driving along good or repaired roads. Your task is to help the Berland government and to find out, which roads need to be repaired.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities and the number of roads in Berland.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>, describing the road from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, than the given road is in a good condition. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">1</span>, then it needs to be repaired.</p><p>It is guaranteed that there is not more than one road between the cities in each direction.</p></div><div class="output-specification"><p>If even after all roads are repaired, it is still impossible to get to some city from the capital, print <span class="tex-span"> - 1</span>. Otherwise, on the first line print the minimum number of roads that need to be repaired, and on the second line print the numbers of these roads, separated by single spaces.</p><p>The roads are numbered starting from <span class="tex-span">1</span> in the order, in which they are given in the input.</p><p>If there are multiple sets, consisting of the minimum number of roads to repair to make travelling to any city from the capital possible, print any of them.</p><p>If it is possible to reach any city, driving along the roads that already are in a good condition, print <span class="tex-span">0</span> in the only output line.</p></div>


## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of cities and the number of roads in Berland.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain three space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 1)</span>, describing the road from city <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to city <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">0</span>, than the given road is in a good condition. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals <span class="tex-span">1</span>, then it needs to be repaired.</p><p>It is guaranteed that there is not more than one road between the cities in each direction.</p>


## Output

<p>If even after all roads are repaired, it is still impossible to get to some city from the capital, print <span class="tex-span"> - 1</span>. Otherwise, on the first line print the minimum number of roads that need to be repaired, and on the second line print the numbers of these roads, separated by single spaces.</p><p>The roads are numbered starting from <span class="tex-span">1</span> in the order, in which they are given in the input.</p><p>If there are multiple sets, consisting of the minimum number of roads to repair to make travelling to any city from the capital possible, print any of them.</p><p>If it is possible to reach any city, driving along the roads that already are in a good condition, print <span class="tex-span">0</span> in the only output line.</p>


## Samples

```input1
3 2
1 3 0
3 2 1

```

```output1
1
2

```






```input2
4 4
2 3 0
3 4 0
4 1 0
4 2 1

```

```output2
-1

```






```input3
4 3
1 2 0
1 3 0
1 4 0

```

```output3
0


```



