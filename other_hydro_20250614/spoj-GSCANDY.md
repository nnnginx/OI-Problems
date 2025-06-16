<p>Jonathan Irvin Gunawan is a very handsome living person. You have to admit it to live in this world.</p>
<p>To become more handsome, Jonathan the Handsome have to collect candies (no relation, indeed). In front of him, there are N candies with different level of sweetness. Jonathan will collect the candies one by one. Jonathan can collect any number of candies, but he must collect the candy in the increasing order of level of sweetness (no two candies will have the same level of sweetness).</p>
<p>Every candy has their own color, which will be represented by a single integer between 0 and 10<sup>9</sup> inclusive.</p>
<p>If Jonathan collects the first candy, or a candy that has different color with the previous candy he take, he will get 1 point.</p>
<p>If Jonathan collects the candy that has the same color with the previous candy, he will get a combo. Combo-x means that he has collected x candies of the same color consecutively. In other words, if he collect a candy and get combo-(x-1) and he collect a candy with the same color again, he will get combo-(x). And then if he collects a candy with different color, the combo will vanish and back to combo- 1.</p>
<p>(Note : previous candy means the last candy he take)</p>
<p>Every time he get combo-x, he will get x points. Jonathan wants to count how many maximum total points he can get. You are a fan of Jonathan the Handsome have to help him.</p>
<h3>Input</h3>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 164px; width: 1px; height: 1px; overflow: hidden;">The first line consists of a single integer T, indicating the number of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 164px; width: 1px; height: 1px; overflow: hidden;">testcases.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 164px; width: 1px; height: 1px; overflow: hidden;">For every testcase, the first line consists of a single integer N.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 164px; width: 1px; height: 1px; overflow: hidden;">The next line consists of N integers, representing the color of the candy given in the increasing level of sweetness, separated by a single space.</div>
<p>The first line consists of a single integer T, indicating the number of testcases.</p>
<p>For every testcase, the first line consists of a single integer N (1 �� N �� 1000).</p>
<p>The next line consists of N integers, representing the color of the candy given in the increasing level of sweetness, separated by a single space.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For every case, output a single integer consist of the maximum total points Jonathan can get.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
4 
1 1 2 1 
4 
1 2 3 1
</pre>
<pre><strong>Output:</strong>
6
4
</pre>
<pre><h3 style="white-space: normal;">Explanation</h3><div>In the first sample, Jonathan chooses not to take the candy with color 2, as he will lose the combo.
In the second sample, he will get a maximum total points if he take all of the candies.</div></pre>