<p>Correct Bracket Sequence (CBS) is a sequence that can be obtained through following rules:
<br>1) An empty string is the CBS. 
<br>2) If A is a CBS, then B = (A) is also a CBS. 
<br>3) If A is a CBS, then B = [A] is also a CBS. 
<br>4) If A and B are CBS, then C = AB is also a CBS.
<br>Length of the CBS is the number of brackets in it, and this number is always even.
<br>Assume that '(' &lt; ')' &lt; '[' &lt; ']'. 
<br>CBS a1a2 ... an is lexicografically smaller than the CBS b1b2 ... bn if and only if there exists an integer i, i &lt;= n, so that aj=bj, for each j, 1 &lt;= j &lt; i and ai &lt; bi.

</p><h3>Illustration</h3>
<p>Enumerate all CBS length 4 in lexicographical order: 
(()), ()(), ()[], ([]), [()], [[]], [](), [][].

</p><h3>Task</h3>
<p> Your task is to find k-th CBS with length n in lexicographical order

</p><h3>Input</h3>
<p>Contains 2 integers n (2..250) and k (1..10^120)

</p><h3>Output</h3>
<p>Print the k-th CBS with length n in lexicographical order
</p><h3>Example</h3>
<pre><b>Input:</b>
4
3
<b>Output:</b>
()[]
</pre>