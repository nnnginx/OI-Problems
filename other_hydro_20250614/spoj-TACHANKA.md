<p>
Our friend Lord Tachanka is on an important mission. He has to reach basecamp quickly. But the evil enemies have stolen many LMG's and have placed them along the way. You'll have to help him out!</p>

<p>Lord Tachanka is initially at the top left corner (1,1) of a rectangular N ¡Á M grid. He needs to reach the bottom right corner (N,M). He can only move down or right. He moves at the speed of 1 cell per second. He has to move every second¡ªthat is, he cannot stop and wait at any cell.</p>

<p>There are K special cells that contain the LMG planted by the enemies. Each LMG has a starting time t and a frequency f. It first fires at time t seconds, followed by another round at time t+f seconds, then at time t+2f seconds ¡­.&nbsp;When a LMG fires, it simultaneously emits four bullets, one in each of the four directions: up, down, left and right.&nbsp;The pulses travel at 1 cell per second.</p>

<p>Suppose a LMG is located at (x,y) with starting time t and frequency f.&nbsp;At time t seconds, it shoots its first set of bullets. The bullets travelling upwards will be at the cell (x,y-s) at time t+s seconds. At this time, the bullets travelling left will be at cell (x-s,y),&nbsp;the bullets travelling right will be at cell (x+s,y) and the bullets travelling down will be at cell (x,y+s).&nbsp;It will fire next at time t+f seconds. If a bullets crosses an edge of the grid, it disappears.&nbsp;The LMG's are numbered 1 to k, and if two bullets from different LMG's happen to meet, the one coming from the higher numbered LMG survives.&nbsp;At any time, if Lord Tachanka and a bullet are in the same cell, he dies.&nbsp;That is the only way bullet interact with Lord Tachanka.&nbsp;</p>

<p>But don't be worried, as you can help the Lord. He can contact his basecamp and can report them the exact position of an LMG, and it will be destroyed by air support. But the war is going on, and you as a commander will have to ensure that minimum missiles are wasted.</p>

<p>Given these, you should find the least time (in seconds) in which Lord Tachanka can reach his basecamp safely.Also calculate the minimum LMG's that are needed to be destroyed so that the Lord can reach the basecamp safely.</p>

<h3>Constraints</h3>
<p>2 &lt;= N, M &lt;= 500</p>
<p>1 &lt;= K &lt;=500</p>

<p>All the frequencies are guaranteed to be integers between 1 and 600, inclusive.</p>
<p>All the starting times are guaranteed to be integers between 0 and 600, inclusive</p>
<p>All the coordinates of the LMGs are guaranteed to be valid cells in the N¡ÁM grid.</p>
<p>No two LMGs will be on the same cell.</p>

<h3>Input</h3>
<p>Line 1: Three space separated integers N, M and K, describing the number of rows and columns in the grid and the number of LMG's, respectively.</p>
<p>Lines 2 to K+1: These lines describe the K LMGs. Each line has four space separated integers.&nbsp;</p>
<p>The first two integers on the line denote the row and column where the LMG is located,&nbsp;</p>
<p>the third integer is its starting time, and the fourth integer is its frequency.</p>
<p>The LMG's are numbered in the order in which it appears in the input, i.e from 1 to k</p>

<h3>Output</h3>
<p>You need to output two integers, the minimum amount of time required for the Lord to reach the basecamp, and the minimum LMG's needed to be destroyed.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
4 4 1
3 2 1 3</pre>

<pre><strong>Output:</strong>
6 0</pre>