<p>Given a set of N integer A = {1, 2, 3, ¡­, N} and a integer S, 
your task is find a way to insert an operator ¡®+¡¯ or ¡®-¡® to every neighbor pair of A, 
that the result of the expression after insert equal to S.</p>

<h3>Input</h3>
<p>A single line, N and S (1 ¡Ü N ¡Ü 500, |S| ¡Ü 125250)</p>

<h3>Output</h3>
<p>If there are way(s) to insert, outputs any of them, otherwise outputs ¡°Impossible¡± (without quotes).</p>

<h3>Example</h3>

<pre><strong>Input:</strong>
9 5

<strong>Output:</strong>
1-2+3-4+5-6+7-8+9</pre>

<pre><strong>Input:</strong>
5 6

<strong>Output:</strong>
Impossible</pre>