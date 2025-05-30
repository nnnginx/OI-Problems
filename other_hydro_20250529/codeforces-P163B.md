## Description

<div><p>As you know, lemmings like jumping. For the next spectacular group jump <span class="tex-span"><i>n</i></span> lemmings gathered near a high rock with <span class="tex-span"><i>k</i></span> comfortable ledges on it. The first ledge is situated at the height of <span class="tex-span"><i>h</i></span> meters, the second one is at the height of <span class="tex-span">2<i>h</i></span> meters, and so on (the <span class="tex-span"><i>i</i></span>-th ledge is at the height of <span class="tex-span"><i>i</i>·<i>h</i></span> meters). The lemmings are going to jump at sunset, and there's not much time left.</p><p>Each lemming is characterized by its climbing speed of <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> meters per minute and its weight <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span>. This means that the <span class="tex-span"><i>i</i></span>-th lemming can climb to the <span class="tex-span"><i>j</i></span>-th ledge in <img align="middle" class="tex-formula" src="./25844/file/E3ppsmci.png" style="max-width: 100.0%;max-height: 100.0%;"> minutes.</p><p>To make the jump beautiful, heavier lemmings should jump from higher ledges: if a lemming of weight <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> jumps from ledge <span class="tex-span"><i>i</i></span>, and a lemming of weight <span class="tex-span"><i>m</i><sub class="lower-index"><i>j</i></sub></span> jumps from ledge <span class="tex-span"><i>j</i></span> (for <span class="tex-span"><i>i</i> &lt; <i>j</i></span>), then the inequation <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i><sub class="lower-index"><i>j</i></sub></span> should be fulfilled.</p><p>Since there are <span class="tex-span"><i>n</i></span> lemmings and only <span class="tex-span"><i>k</i></span> ledges (<span class="tex-span"><i>k</i> ≤ <i>n</i></span>), the <span class="tex-span"><i>k</i></span> lemmings that will take part in the jump need to be chosen. The chosen lemmings should be distributed on the ledges from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i></span>, one lemming per ledge. The lemmings are to be arranged in the order of non-decreasing weight with the increasing height of the ledge. In addition, each lemming should have enough time to get to his ledge, that is, the time of his climb should not exceed <span class="tex-span"><i>t</i></span> minutes. The lemmings climb to their ledges all at the same time and they do not interfere with each other.</p><p>Find the way to arrange the lemmings' jump so that time <span class="tex-span"><i>t</i></span> is minimized.</p></div><div class="input-specification"><p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">4</sup></span>) — the total number of lemmings, the number of ledges and the distance between adjacent ledges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> is the weight of <span class="tex-span"><i>i</i></span>-th lemming.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the speed of <span class="tex-span"><i>i</i></span>-th lemming.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>k</i></span> different numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of the lemmings who go to ledges at heights <span class="tex-span"><i>h</i>, 2<i>h</i>, ..., <i>kh</i></span>, correspondingly, if the jump is organized in an optimal way. If there are multiple ways to select the lemmings, pick any of them.</p></div>


## Input

<p>The first line contains space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> and <span class="tex-span"><i>h</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10<sup class="upper-index">4</sup></span>) — the total number of lemmings, the number of ledges and the distance between adjacent ledges.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>m</i><sub class="lower-index">1</sub>, <i>m</i><sub class="lower-index">2</sub>, ..., <i>m</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>m</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>m</i><sub class="lower-index"><i>i</i></sub></span> is the weight of <span class="tex-span"><i>i</i></span>-th lemming.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>v</i><sub class="lower-index">1</sub>, <i>v</i><sub class="lower-index">2</sub>, ..., <i>v</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> is the speed of <span class="tex-span"><i>i</i></span>-th lemming.</p>


## Output

<p>Print <span class="tex-span"><i>k</i></span> different numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> — the numbers of the lemmings who go to ledges at heights <span class="tex-span"><i>h</i>, 2<i>h</i>, ..., <i>kh</i></span>, correspondingly, if the jump is organized in an optimal way. If there are multiple ways to select the lemmings, pick any of them.</p>


## Samples

```input1
5 3 2
1 2 3 2 1
1 2 1 2 10

```

```output1
5 2 4

```






```input2
5 3 10
3 4 3 2 1
5 4 3 2 1

```

```output2
4 3 1

```




## Note

<p>Let's consider the first sample case. The fifth lemming (speed 10) gets to the ledge at height 2 in <img align="middle" class="tex-formula" src="./25844/file/vMq3idCo.png" style="max-width: 100.0%;max-height: 100.0%;"> minutes; the second lemming (speed 2) gets to the ledge at height 4 in 2 minutes; the fourth lemming (speed 2) gets to the ledge at height 6 in 3 minutes. All lemmings manage to occupy their positions in 3 minutes. </p>

