<p>We say that an integer sequence a<sub>1</sub>,&nbsp;a<sub>2</sub>,&nbsp;... , a<sub>n</sub> is k-even if the sum of any k consecutive terms of the sequence is even.</p>
<p>For a given sequence we would like to find out how many of its terms need to be changed so that the sequence becomes k-even.</p>
<h3>Input</h3>
<p>The first line of input contains two integers n and k (1 ¡Ü k ¡Ü n ¡Ü 10<sup>6</sup>). The second line contains a sequence composed of n integers a<sub>1</sub>,&nbsp;a<sub>2</sub>,&nbsp;... , a<sub>n</sub>. For each of the a<sub>i</sub>'s it holds that 0 ¡Ü a<sub>i</sub>&nbsp;¡Ü 10<sup>9</sup>.</p>
<h3>Output</h3>
<p>The only line of output should hold one integer: the minimum number of terms of the sequence that need to be changed so that it becomes k-even.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8 3
1 2 3 4 5 6 7 8

<strong>Output:</strong>
3
</pre>
<pre><strong>Input:</strong>
8 3
2 4 2 4 2 4 2 4

<strong>Output:</strong>
0
</pre>