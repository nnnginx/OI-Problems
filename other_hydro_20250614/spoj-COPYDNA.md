<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/COPYDNA/en/">English</a></td> 
<td width="50%"><a href="/problems/COPYDNA/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>
Evolution is a seemingly random process which works in a way
which resembles certain approaches we use to get approximate
solutions to hard combinatorial problems. You are now to do
something completely different.
</p>
<p>
Given a DNA string S from the alphabet {A,C,G,T}, find the
minimal number of copy operations needed to create another string
T. You may reverse the strings you copy, and copy both from S
and the pieces of your partial T. You may put these pieces together
at any time. You may only copy contiguous parts of your partial
T, and all copied strings must be used in your final T. </p>
<p>Example:
From S = ¡°ACTG¡± create T = ¡°GTACTATTATA¡±</p>
<ol>
<li>Get GT......... by copying and reversing ¡°TG¡± from S.</li>
<li>Get GTAC....... by copying ¡°AC¡± from S.</li>
<li>Get GTAC...TA.. by copying ¡°TA¡± from the partial T.</li>
<li>Get GTAC...TAAT by copying and reversing ¡°TA¡± from the partial T.</li>
<li>Get GTACAATTAAT by copying ¡°AAT¡± from the partial T.</li>
</ol>
<h3>Input</h3>
<p>
The first line of input gives a single integer, 1 ¡Ü t ¡Ü 100, the number of test cases. Then
follow, for each test case, a line with the string S of length 1 ¡Ü m ¡Ü 18, and a line with
the string T of length 1 ¡Ü n ¡Ü 18.
</p>

<h3>Output</h3>
<p>Output for each test case the number of copy operations needed to create T from S, or
¡°impossible¡± if it cannot be done.
</p>

<h3>Example</h3>
<pre><b>Input</b>
5
ACGT
GTAC
A
C
ACGT
TGCA
ACGT
TCGATCGA
A
AAAAAAAAAAAAAAAAAA

<b>Output</b>
2
impossible
1
4
6
</pre>