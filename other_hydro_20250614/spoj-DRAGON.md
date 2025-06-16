<p>Hydra is some very greedy animal. A hydra has 9 heads when he is born, and many more new heads will come out when he grows up. Of course, some old heads will break off because of caducidy.</p>
<p>One day, a hydra with M heads finds a tree with N fruits on it. He is very delighted and wants to eat this tree instantly. Since he has M heads, he must divide these N fruit into M groups, each group contains at least 1 fruit, and each head will eat a group of fruits.</p>
<p>The biggest head among the M heads is named "Boss", it must eat neither more nor less than K fruits, and, in the nature of things, the biggest fruit included. These fruits are connected by N-1 branches, and there exists a path made up with branches between each pair of fruit.</p>
<p>If two fruit connected by a single branch is put in different groups, the corresponding two heads will break the branch and eat the two fruits, otherwise the corresponding head will eat the two fruits without breaking the branch. Eating branches is not very comfortable of course, so every branch has a weight of illness, and the weight of illness of this hydra is the sum of the weights of illness of all brances he has eaten.</p>
<p>Your task is to help the hydra to minimize his weight of illness.</p>
<p>The picture below is an example.</p>
<p><img src="../../../content/john_jones:dragon.jpg" alt=""></p>
<p>N=8,M=2,K=4.The bigger head eats 4 fruits(full points), the smaller head eats 4 fruits(empty points). The branch signed by a thin segment is eaten by the hydra.</p>
<h3>Input</h3>
<p>Ten test cases(Given one after another, you have to process all!). For each test case the first line contains 3 integers N(1&lt;=N&lt;=300),M(2&lt;=M&lt;=N),K(1&lt;=K&lt;=N), separated by single spaces. The N fruits are numbered 1..N, and the biggest fruit is always numbered 1. N-1 lines follow, each contains 3 integers i,j,k separated by spaces denoted that there is a branch between fruit i(1&lt;=i&lt;=N) and fruit j(1&lt;=j&lt;=N) and the weight of illness of this branch is k(0&lt;=k&lt;=100000).</p>
<h3>Output</h3>
<p>Ten lines, each contains a single integer - the minimum weight of illness of the hydra. If we can't divide the fruit into M groups, output "-1"(without quotes).</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
8 2 4
1 2 20
1 3 4 
1 4 13
2 5 10
2 6 12
3 7 15
3 8 5
[and 9 test cases more]

<strong>Output:</strong>
4
[and 9 test cases more]
</pre>
<h3>Link</h3>
<p>After solving this problem you can try the problem <a href="http://www.spoj.com/problems/DRAGON2">DRAGON2</a>.</p>