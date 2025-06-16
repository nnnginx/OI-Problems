<p>Ada the Ladybug came home with difficult homework. Since she is very skilled mathematician, she already deduced, how to count the answer for N. Consider all numbers <strong>K</strong>(in range <strong>2 ¡Ü K ¡Ü N</strong>), for which it is true that <em>gcd(N,K)==1</em> and add <em>gcd(N,K-1)</em> to sum. What is the sum?</p>
<p>A little bit more formally, find: ¡Æ gcd(K-1,N), for K ¡Ê [2,N] where gcd(N,K)==1</p>
<p>Anyway the numbers are too large, so she can't do that without your help. Can you help her?</p>
<h3>Input</h3>
<p>The first line contains <strong>1 ¡Ü T ¡Ü 1000 </strong>, number of test-cases.</p>
<p>Each of following <strong>T</strong> lines contains <strong> 2 ¡Ü N ¡Ü     10<sup>18</sup></strong>, number for which ada wants the answer.</p>
<h3>Output</h3>
<p>For each test case, print the sum of deduced formula.</p>
<h3>Example Input</h3>
<pre>11
2
5
6
7
8
10
50
100
1000
524288
945406969379503350
</pre>
<h3>Example Output</h3>
<pre>0
3
2
5
8
6
70
260
5400
4718592
1381966975399059833610
</pre>