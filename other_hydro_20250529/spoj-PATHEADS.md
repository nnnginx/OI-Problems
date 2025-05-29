<p>It's Bessie's birthday and time for party games! Bessie has instructed the N (1 ¡Ü N ¡Ü 100,000) cows conveniently numbered 1..N to sit in a circle (so that cow i [except at the ends] sits next to cows i-1 and i+1; cow N sits next to cow 1). Meanwhile, Farmer John fills a barrel with one billion slips of paper, each containing some integer in the range 1..1,000,000.</p>
<p>Each cow i then draws a number A<sub>i</sub> (1 ¡Ü A<sub>i</sub> ¡Ü 1,000,000) (which is not necessarily unique, of course) from the giant barrel.  Taking turns, each cow i then takes a walk around the circle and pats the heads of all other cows j such that her number A<sub>i</sub> is exactly divisible by cow j's number A<sub>j</sub>; she then sits again back in her original position.</p>
<p>The cows would like you to help them determine, for each cow, the number of other cows she should pat.</p>
<h3>Input</h3>
<ul>
<li>Line 1: A single integer: N.</li>
<li>Lines 2..N+1: Line i+1 contains a single integer: A<sub>i</sub>.</li>
</ul>
<h3>Output</h3>
<ul>
<li>Lines 1..N: On line i, print a single integer that is the number of other cows patted by cow i.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong>
5
2
1
2
3
4

<strong>Output:</strong>
2
0
2
1
3
</pre>
<p>The first cow pats the second and third cows; the second cows pats no cows; etc.</p>