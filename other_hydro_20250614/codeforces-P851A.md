## Description

<div><p>Arpa is researching the Mexican wave.</p><p>There are <span class="tex-span"><i>n</i></span> spectators in the stadium, labeled from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. They start the Mexican wave at time <span class="tex-span">0</span>. </p><ul> <li> At time <span class="tex-span">1</span>, the first spectator stands. </li><li> At time <span class="tex-span">2</span>, the second spectator stands. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>k</i></span>, the <span class="tex-span"><i>k</i></span>-th spectator stands. </li><li> At time <span class="tex-span"><i>k</i> + 1</span>, the <span class="tex-span">(<i>k</i> + 1)</span>-th spectator stands and the first spectator sits. </li><li> At time <span class="tex-span"><i>k</i> + 2</span>, the <span class="tex-span">(<i>k</i> + 2)</span>-th spectator stands and the second spectator sits. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>n</i></span>-th spectator stands and the <span class="tex-span">(<i>n</i> - <i>k</i>)</span>-th spectator sits. </li><li> At time <span class="tex-span"><i>n</i> + 1</span>, the <span class="tex-span">(<i>n</i> + 1 - <i>k</i>)</span>-th spectator sits. </li><li> <span class="tex-span">...</span> </li><li> At time <span class="tex-span"><i>n</i> + <i>k</i></span>, the <span class="tex-span"><i>n</i></span>-th spectator sits. </li></ul><p>Arpa wants to know how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i> &lt; <i>n</i> + <i>k</i></span>).</p></div><div class="output-specification"><p>Print single integer: how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>t</i> &lt; <i>n</i> + <i>k</i></span>).</p>

## Output

<p>Print single integer: how many spectators are standing at time <span class="tex-span"><i>t</i></span>.</p>

## Samples

```input1
10 5 3

```

```output1
3

```






```input2
10 5 7

```

```output2
5

```






```input3
10 5 12

```

```output3
3

```




## Note

<p>In the following a sitting spectator is represented as <span class="tex-font-style-tt">-</span>, a standing spectator is represented as <span class="tex-font-style-tt">^</span>.</p><ul> <li> At <span class="tex-span"><i>t</i> = 0 </span> <span class="tex-font-style-tt">----------</span> <img align="middle" class="tex-formula" src="./28732/file/rVPvDj7d.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 0. </li><li> At <span class="tex-span"><i>t</i> = 1 </span> <span class="tex-font-style-tt">^---------</span> <img align="middle" class="tex-formula" src="./28732/file/n38TJK2o.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 1. </li><li> At <span class="tex-span"><i>t</i> = 2 </span> <span class="tex-font-style-tt">^^--------</span> <img align="middle" class="tex-formula" src="./28732/file/2F8CZf7l.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 2. </li><li> At <span class="tex-span"><i>t</i> = 3 </span> <span class="tex-font-style-tt">^^^-------</span> <img align="middle" class="tex-formula" src="./28732/file/6D9rLe8w.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 3. </li><li> At <span class="tex-span"><i>t</i> = 4 </span> <span class="tex-font-style-tt">^^^^------</span> <img align="middle" class="tex-formula" src="./28732/file/IsPQnGyM.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 4. </li><li> At <span class="tex-span"><i>t</i> = 5 </span> <span class="tex-font-style-tt">^^^^^-----</span> <img align="middle" class="tex-formula" src="./28732/file/CTWvGGeD.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 6 </span> <span class="tex-font-style-tt">-^^^^^----</span> <img align="middle" class="tex-formula" src="./28732/file/KXqggvyG.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 7 </span> <span class="tex-font-style-tt">--^^^^^---</span> <img align="middle" class="tex-formula" src="./28732/file/ldnJq51I.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 8 </span> <span class="tex-font-style-tt">---^^^^^--</span> <img align="middle" class="tex-formula" src="./28732/file/M7tHY1sf.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 9 </span> <span class="tex-font-style-tt">----^^^^^-</span> <img align="middle" class="tex-formula" src="./28732/file/tq8OQn1Z.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 10</span> <span class="tex-font-style-tt">-----^^^^^</span> <img align="middle" class="tex-formula" src="./28732/file/ev5MeE3i.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 5. </li><li> At <span class="tex-span"><i>t</i> = 11</span> <span class="tex-font-style-tt">------^^^^</span> <img align="middle" class="tex-formula" src="./28732/file/y2F03J3W.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 4. </li><li> At <span class="tex-span"><i>t</i> = 12</span> <span class="tex-font-style-tt">-------^^^</span> <img align="middle" class="tex-formula" src="./28732/file/uNN6TxH2.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 3. </li><li> At <span class="tex-span"><i>t</i> = 13</span> <span class="tex-font-style-tt">--------^^</span> <img align="middle" class="tex-formula" src="./28732/file/TbYp7zlB.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 2. </li><li> At <span class="tex-span"><i>t</i> = 14</span> <span class="tex-font-style-tt">---------^</span> <img align="middle" class="tex-formula" src="./28732/file/JW9cMcOt.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 1. </li><li> At <span class="tex-span"><i>t</i> = 15</span> <span class="tex-font-style-tt">----------</span> <img align="middle" class="tex-formula" src="./28732/file/epFXDmSg.png" style="max-width: 100.0%;max-height: 100.0%;"> number of standing spectators = 0. </li></ul>
