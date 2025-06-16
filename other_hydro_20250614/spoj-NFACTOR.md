<p>A number is called&nbsp;<strong>n</strong>-factorful if it has exactly&nbsp;<strong>n</strong>&nbsp;distinct prime factors. Given positive integers&nbsp;<strong>a</strong>,&nbsp;<strong>b</strong>, and&nbsp;<strong>n</strong>, your task is to find the number of integers between&nbsp;<strong>a</strong>&nbsp;and&nbsp;<strong>b</strong>, inclusive, that are&nbsp;<strong>n</strong>-factorful. We consider 1 to be 0-factorful.</p>

<h3>Input</h3>
<p>Your input will consist of a single integer&nbsp;<strong>T</strong>&nbsp;followed by a newline and&nbsp;<strong>T</strong>&nbsp;test cases. Each test cases consists of a single line containing integers&nbsp;<strong>a</strong>,&nbsp;<strong>b</strong>, and&nbsp;<strong>n</strong>&nbsp;as described above.</p>

<p><strong>T</strong>&nbsp;&gt; 10000<br>1 ¡Ü&nbsp;<strong>a</strong>&nbsp;¡Ü&nbsp;<strong>b</strong>&nbsp;¡Ü 10<span style="font-size: xx-small;"><sup>6</sup></span><br>0 ¡Ü&nbsp;<strong>n</strong>&nbsp;¡Ü 10</p>

<h3>Output</h3>
<p>Output for each test case one line containing the number of&nbsp;<strong>n</strong>-factorful integers in [<strong>a</strong>,&nbsp;<strong>b</strong>].</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5
1 3 1
1 10 2
1 10 3
1 100 3
1 1000 0

<strong>Output:</strong>
2
2
0
8
1</pre>