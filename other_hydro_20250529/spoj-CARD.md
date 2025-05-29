<p>
Zenek is a well known (at least in Byteotia) card-sharper. He spent most of his best years practicing one card shuffle with his deck of <b>n</b> cards, which for simplicity we will call 1, 2, ..., <b>n</b>. Unfortunately, it turns out that knowing this one card shuffle <b>a</b> is not enough to earn a good living. To become rich and famous Zenek needs to know <b>k</b> shuffles <b>c<sub>1</sub></b>, ..., <b>c<sub>k</sub></b>. As he doesn't have  enough time to learn all of them, he decided to learn only one shuffle <b>b</b> so that using both <b>a</b> and <b>b</b> he will be able to perform as many of <b>c<sub>i</sub></b> as it is possible.
</p>

<p>
Each shuffle is described by <b>n</b> numbers <b>t<sub>1</sub></b>, <b>t<sub>2</sub></b>, ..., <b>t<sub>n</sub></b>. Such description means that after performing shuffle, card that was originally at position <b>i</b> will be at position <b>t<sub>i</sub></b>.
</p>

<h3>Task</h3>
<p>Find shuffle <b>b</b> maximizing number of shuffles that can be performed.</p>

<h3>Input</h3>
<p>First line contains <b>n</b> (2 ¡Ü <b>n</b> ¡Ü 52). Second line contains <b>n</b> numbers <b>a<sub>1</sub></b>, <b>a<sub>2</sub></b>, ..., <b>a<sub>n</sub></b> describing shuffle that Zenek already knows. Third line contains <b>k</b> (2 ¡Ü <b>k</b> ¡Ü 6). <b>i</b>-th of the next <b>k</b> lines contains description of <b>c<sub>i</sub></b>.
</p>

<h3>Output</h3>
<p>First line contains description of the shuffle <b>b</b> that Zenek should learn. <b>i</b>-th of the next <b>k</b> lines contains:</p>
<ul>
<li> <code>-1</code> when it is not possible to perform <b>c<sub>i</sub></b> using only <b>a</b> and <b>b</b> </li>
<li> <b>m</b>, <b>r<sub>1</sub></b>, <b>r<sub>2</sub></b>, ..., <b>r<sub>m</sub></b> (0 ¡Ü <b>m</b> ¡Ü 500000, 0 ¡Ü <b>r<sub>i</sub></b> ¡Ü 10<sup>6</sup>) meaning that applying <b>a</b> <b>r<sub>1</sub></b> times, then <b>b</b> <b>r<sub>2</sub></b> times, then <b>a</b> <b>r<sub>3</sub></b> times and so on is the same as applying shuffle <b>c<sub>i</sub></b> once. </li>
</ul>

<h3>Examples</h3>
<p><strong>Input</strong></p>
<pre>5
2 3 4 5 1
3
1 3 2 4 5
1 2 3 4 5
5 4 3 2 1
</pre>
<p><strong>Output</strong></p>
<pre>2 1 3 4 5
3 4 1 1
0
9 1 1 3 1 4 1 1 1 1
</pre>
<p><strong>Input</strong></p>
<pre>5
1 2 3 4 5
3
1 3 2 4 5
5 4 3 2 1
1 2 5 4 3
</pre>
<p><strong>Output</strong></p>
<pre>1 3 2 4 5
2 0 1
-1
-1
</pre>