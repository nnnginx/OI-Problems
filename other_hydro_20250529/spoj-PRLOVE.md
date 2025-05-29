<script type="text/x-mathjax-config">
MathJax.Hub.Config({
  tex2jax: {
    inlineMath: [['$','$'], ['\\(','\\)']],
    skipTags: ["script","noscript","style","textarea","code"]
  }
});
</script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>


<p>Alice has a problem. She loves Bob but is unable to face up to him. So she decides to send a letter to Bob expressing her feelings. She wants to send it from her computer to Bob's computer through the internet.</p>

<p>The internet consists of $N$ computers, numbered from $1$ to $N$. Alice's computer has the number $1$ and Bob's computer has the number $N$. </p>

<p>Due to some faulty coding, the computers start behaving in unexpected ways. On recieving the file, computer $i$ will forward it to computer $j$ with probability $P_{ij}$. The time taken to transfer the file from computer $i$ to computer $j$ is $T_{ij}$.</p>

<p>Find the expected time before Bob finds out about Alice's undying love for him.</p>

<p><strong>Note:</strong>
Once the letter is recieved by Bob's computer, his computer will just deliver it to Bob and stop forwarding it.</p>

<h3>Input</h3>

<p>First line contains $T$, the total test cases.</p>

<p>Each test case looks as follows:</p>

<p>First line contains $N$, the total number of computers in the network.</p>

<p>The next $N$ lines contain $N$ numbers each. The $j$'th number on the $i$'th line is the value $P_{ij}$ in percents.</p>

<p>The next $N$ lines contain $N$ numbers each. The $j$'th number on the $i$'th line is the value $T_{ij}$.</p>

<h3>Output</h3>

<p>Output a single line with a real number - The expected time of the transfer.</p>

<p>Your output will be considered correct if each number has an absolute or relative error less than $10^{-6}$. </p>

<h3>Constraints</h3>

<p>$N \le 100$</p>
<p>$T \le 5$</p>
<p>For all $i$, $P_{i1} + P_{i2} + \ldots + P_{iN} = 100$</p>
<p>$P_{NN} = 100$</p>
<p>For all $i$, $j$, $0 \le T_{ij} \le 10000$</p>

<p>You can safely assume that from every computer, the probability of eventually reaching Bob's computer is greater than $0$.</p>

<h3>Example</h3>

<pre><strong>Sample Input:</strong>
2
4
0 50 50 0
0 0 0 100
0 0 0 100
0 0 0 100
0 2 10 0
0 0 0 0
0 0 0 0
0 0 0 0
2
99 1
0 100
10 2
0 0</pre>

<pre><strong>Sample Output:</strong>
6.000000
992.000000</pre>