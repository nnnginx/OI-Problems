<p>Given a sequence a1, a2,..., an&nbsp;and a integer S, 
your task is find a way to insert an operator ¡®<tt>+</tt>¡¯ , ¡®<tt>-</tt>¡®,&nbsp;¡®<tt>.</tt>¡®,&nbsp;¡®<tt>~</tt>¡®&nbsp;
to every neighbor pair of A, that the result of the expression after insert equal to S.</p>

<p><strong>Note that :</strong>
</p><ul>
  <li><tt>a . b = a + 2 * b</tt></li>
  <li><tt>a ~ b = a - 2 * b</tt></li>
</ul>
<p></p>

<h3>Input</h3>
<p>First line : N and S (2 ¡Ü N ¡Ü 22, |S| ¡Ü 5 * 10<sup>16</sup>)</p>
<p>Second line : N integers,&nbsp;a1, a2,..., an &nbsp;(|ai|&nbsp;¡Ü 10<sup>15</sup>)</p>

<h3>Output</h3>
<p>If there are way(s) to insert, output any of them, otherwise output ¡°Impossible¡± (without quotes).</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
9 5
1 2 3 4 5 6 7 8 9

<strong>Output:</strong>
-~~~++++</pre>

<pre><strong>Input:</strong>
3 -1
-2 5 7

<strong>Output:</strong>
Impossible</pre>

<p><strong>Details:</strong></p>
<p>In first test case : 1 - 2 - 2 * 3 - 2 * 4 - 2 * 5 + 6 + 7 + 8 + 9 = 5</p>
<p>You may want to try another version <a href="../../problems/BLOPER">here</a>.</p>