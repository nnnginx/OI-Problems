## Description

<div><p>The polar bears are going fishing. They plan to sail from <span class="tex-span">(<i>s</i><sub class="lower-index"><i>x</i></sub>, <i>s</i><sub class="lower-index"><i>y</i></sub>)</span> to <span class="tex-span">(<i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub>)</span>. However, the boat can only sail by wind. At each second, the wind blows in one of these directions: east, south, west or north. Assume the boat is currently at <span class="tex-span">(<i>x</i>, <i>y</i>)</span>.</p><ul> <li> If the wind blows to the east, the boat will move to <span class="tex-span">(<i>x</i> + 1, <i>y</i>)</span>. </li><li> If the wind blows to the south, the boat will move to <span class="tex-span">(<i>x</i>, <i>y</i> - 1)</span>. </li><li> If the wind blows to the west, the boat will move to <span class="tex-span">(<i>x</i> - 1, <i>y</i>)</span>. </li><li> If the wind blows to the north, the boat will move to <span class="tex-span">(<i>x</i>, <i>y</i> + 1)</span>. </li></ul><p>Alternatively, they can hold the boat by the anchor. In this case, the boat stays at <span class="tex-span">(<i>x</i>, <i>y</i>)</span>. Given the wind direction for <span class="tex-span"><i>t</i></span> seconds, what is the earliest time they sail to <span class="tex-span">(<i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub>)</span>?</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>t</i>, <i>s</i><sub class="lower-index"><i>x</i></sub>, <i>s</i><sub class="lower-index"><i>y</i></sub>, <i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>s</i><sub class="lower-index"><i>x</i></sub>, <i>s</i><sub class="lower-index"><i>y</i></sub>, <i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The starting location and the ending location will be different.</p><p>The second line contains <span class="tex-span"><i>t</i></span> characters, the <span class="tex-span"><i>i</i></span>-th character is the wind blowing direction at the <span class="tex-span"><i>i</i></span>-th second. It will be one of the four possibilities: "E" (east), "S" (south), "W" (west) and "N" (north).</p></div><div class="output-specification"><p>If they can reach <span class="tex-span">(<i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub>)</span> within <span class="tex-span"><i>t</i></span> seconds, print the earliest time they can achieve it. Otherwise, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p></div>


## Input

<p>The first line contains five integers <span class="tex-span"><i>t</i>, <i>s</i><sub class="lower-index"><i>x</i></sub>, <i>s</i><sub class="lower-index"><i>y</i></sub>, <i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 10<sup class="upper-index">5</sup>,  - 10<sup class="upper-index">9</sup> ≤ <i>s</i><sub class="lower-index"><i>x</i></sub>, <i>s</i><sub class="lower-index"><i>y</i></sub>, <i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. The starting location and the ending location will be different.</p><p>The second line contains <span class="tex-span"><i>t</i></span> characters, the <span class="tex-span"><i>i</i></span>-th character is the wind blowing direction at the <span class="tex-span"><i>i</i></span>-th second. It will be one of the four possibilities: "E" (east), "S" (south), "W" (west) and "N" (north).</p>


## Output

<p>If they can reach <span class="tex-span">(<i>e</i><sub class="lower-index"><i>x</i></sub>, <i>e</i><sub class="lower-index"><i>y</i></sub>)</span> within <span class="tex-span"><i>t</i></span> seconds, print the earliest time they can achieve it. Otherwise, print "<span class="tex-font-style-tt">-1</span>" (without quotes).</p>


## Samples

```input1
5 0 0 1 1
SESNW

```

```output1
4

```






```input2
10 5 3 3 6
NENSWESNEE

```

```output2
-1

```




## Note

<p>In the first sample, they can stay at seconds <span class="tex-span">1</span>, <span class="tex-span">3</span>, and move at seconds <span class="tex-span">2</span>, <span class="tex-span">4</span>.</p><p>In the second sample, they cannot sail to the destination.</p>

