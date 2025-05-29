<p>CS&amp;T, the well-known cellphone company, is going to set some new service stations among n possible ones, which are numbered 1,2,...,n. The costs of setting these stations are known as P1,P2,..,Pn. Also the company has made a survey among the cellphone users, and now they know that there are m user groups numbered 1,2,...,m, which will communicate by service station Ai and Bi, and the company can profit Ci.</p>
<p>Now CS&amp;T wants to know which service stations are to be set that the company will profit most.</p>
<h3>Input</h3>
<pre>T [The number of tests]
n m [n&lt;=5000 m&lt;=50000]
P1 P2 P3 ... Pn [Pi&lt;=100]
A1 B1 C1 
A2 B2 C2
...
Am Bm Cm [1&lt;=Ai,Bi&lt;=n, Ci&lt;=100]
[other tests]
<p>At least 80% of the tests satisfy that n&lt;=200, m&lt;=1000.</p>
</pre>
<h3>Output</h3>
<pre>MaximumProfit
[other tests]
</pre>
<h3>Example</h3>
<pre><b>Input:</b>
1
5 5
1 2 3 4 5
1 2 3
2 3 4
1 3 3
1 4 2
4 5 3

<b>Output:</b>
4
<b>Hints:</b>
The service stations to be set are 1,2,3.
</pre>