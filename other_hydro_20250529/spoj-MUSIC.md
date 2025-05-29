<p>Bessie the cow used to write musical melody. A musical melody is
represented as a sequence of N (1 &lt;= N &lt;= 100,000) notes numbered 1..N.
Note i is  represented by the integer A<sub>i</sub> (-10,000 &lt;= A<sub>i</sub> &lt;= 10,000).</p>

<p>To Bessie's cow-like mind, a musical melody is called 'perfect' if and only
if the sum of all the notes in any of its consecutive subsequences is
strictly positive.</p>

<p>For a given musical melody, Bessie wants to make it perfect, but she wants
to change the melody as little as possible.</p>

<p>Thus, to perfect the melody, she repeatedly chooses a consecutive
subsequence of the melody, [x, y] (1 &lt; x &lt;= y &lt; N), whose sum S is
negative. Then she adds S to both A<sub>x-1</sub> and A<sub>y+1</sub>, while subtracting S from
both A<sub>x</sub> and A<sub>y</sub>. (It is possible to subtract from the same note twice if x
= y.)</p>

<p>Given a musical melody, compute the minimum number of steps to make the
melody perfect.</p>

<h3>Input</h3>

<p>* Line 1: The single integer N.</p>

<p>* Lines 2..N+1: Line i+1 contains the single integer A<sub>i</sub>.</p>

<h3>Output</h3>

<p>* Line 1: A single integer that represents the minimum number of steps
        needed to make the given musical melody perfect. If there are
        no solutions, output -1 instead.</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
13
-3
-4
-5
62

<b>Output:</b>
2
</pre>
<b>Explanation</b>
<p>There is a musical melody with length of 5. The notes are (13, -3, -4, -5, 62).</p>
<p>First, we choose the range [2, 4]; its sum is (-3) + (-4) + (-5) = -12.
After the first step, the melody becomes (1, 9, -4, 7, 50). Second, we
choose the range [3, 3], whose sum is -4, and the melody after the second
step becomes (1, 5, 4, 3, 50). The melody is perfect now.</p>
<b>Warning: large input/output data, be careful with certain languages</b>