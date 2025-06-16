<p>You are given sequence <em>A<sub>1</sub>, A<sub>2</sub>, ... A<sub>n</sub></em>&nbsp;and&nbsp;integer <em>k</em>. For each integer <em>i</em> <em>(0 ¡Ü i &lt; k)</em> find such <strong>nonempty</strong> subsequence of <em>A</em> so that sum of numbers in this subsequence is maximal possible and remainder of integer division of this sum by <em>k</em> is equal to <em>i</em>.</p>
<h3>Input</h3>
<p>In first line numbers <em>n</em> and <em>k (1 ¡Ü n ¡Ü 10<sup>6</sup>, 1 ¡Ü k ¡Ü 200)</em>.</p>
<p>In second line: <em>n</em> numbers representing sequence <em>A (1 ¡Ü A<sub>i</sub>&nbsp;¡Ü 10<sup>9</sup>)</em>.&nbsp;</p>
<h3>Output</h3>
<p>Print <em>k</em> numbers in one line. <em>i</em>'th number represent sum of numbers in subsequence for number <em>i - 1</em>. If there is no such subsequence print -1.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
6 5
2 8 10 44 15 32
<strong>Output:</strong>
65 111 77 103 109
</pre>