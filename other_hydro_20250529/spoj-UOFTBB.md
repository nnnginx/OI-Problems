<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The Bloons (not to be confused with balloons) are attacking! They are attempting to navigate your course of $L$ ($1 \leq L \leq 1000$) cells, laid out in a row and numbered from $1$ to $L$. You don't know what they'll do to you if they manage reach the end, and you don't want to find out! To that end, you've constructed some defensive towers along the course. You might say that this is a Bloons Tower Defense.</p>
<p>There are $N$ ($1 \leq N \leq 1000$) towers ready to take out any Bloons that get close. The $i$th tower is located next to cell $C_i$ ($1 \leq C_i \leq L$), and can launch darts at any Bloons that are no more than $R_i$ ($0 \leq R_i \leq 1000$) cells away - that is, Bloons in cells $C_i-R_i$ to $C_i+R_i$, inclusive. Every second, it will do $D_i$ ($1 \leq D_i \leq 10^9$) HP worth of damage to any Bloons in this range.</p>
<p>$M$ ($1 \leq M \leq 1000$) Bloons will attempt to float through your course, one after another. The $i$th Bloon begins with $H_i$ ($1 \leq H_i \leq 10^9$) HP, and will pop as soon as it has taken at least that much damage in total. Each Bloon starts in cell 1, and moves along the course at a speed of 1 cell per second. If a Bloon moves past cell $L$, it safely exits the course and can no longer be popped.</p>
<p>There are $T$ ($1 \leq T \leq 20$) scenarios as described above. For each, you'd like to determine how far along the course each of the $M$ Bloons will make it.</p>
<h3>Input</h3>
<p>First line: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>First line: 2 integers, $L$ and $N$</p>
<p>Next $N$ lines: 3 integers, $C_i$, $R_i$, and $D_i$, for $i = 1..N$</p>
<p>Next line: 1 integer, $M$</p>
<p>Next $M$ lines: 1 integer, $H_i$, for $i = 1..M$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>$M$ lines: If the $i$th Bloon will survive the course, the string "Bloon leakage" (without quotes) - otherwise, 1 integer, the furthest cell which the $i$th Bloon will reach, for $i = 1..M$</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>10 3<br>3 3 1<br>4 0 4<br>10 2 2<br>4<br>1<br>20<br>9<br>11</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>Bloon leakage<br>5<br>8</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>The following diagram illustrates which cells each tower can hit:</p>
<p><img src="../../../content/sourspinach:uoftbb.png" alt=""></p>
<p>The first Bloon, having only 1 HP, will go down to the first tower in cell 1.</p>
<p>The second Bloon will manage to clear the course, surviving past cell 10 with 4 HP remaining.</p>
<p>The third Bloon will lose its final HP while at cell 5, having taken 5 damage from the first tower, and 4 from the second.</p>
<p>The final Bloon will survive past cell 6 with 1 HP remaining, but will then go down at cell 8 when it takes 2 damage from the third tower.</p>