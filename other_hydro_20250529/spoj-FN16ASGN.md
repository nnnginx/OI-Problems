<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>The Innovative Consumer Products Company (ICPC) is planning     to start a top-secret project. This project consists of     $s$ subprojects. There     will be $b \ge s$ branches     of ICPC involved in this project and ICPC wants to assign each     branch to one of the subprojects. In other words, the branches     will form $s$ disjoint     groups, with each group in charge of a subproject.</p>
<p>At the end of each month, each branch will send a message to     every other branch in its group (a different message to each     branch). ICPC has a particular protocol for its communications.     Each branch $i$ has a     secret key $k_ i$ known     only to the branch and the ICPC headquarters. Assume branch     $i$ wants to send a     message to branch $j$.     Branch $i$ encrypts its     message with its key $k_     i$. A trusted courier picks up this message from this     branch and delivers it to the ICPC headquarters. Headquarters     decrypts the message with key $k_     i$ and re-encrypts it with key      $k_ j$. The courier then delivers this     newly encrypted message to branch      $j$, which decrypts it with its own     key $k_ j$. For security     reasons, a courier can carry only one message at a time.</p>
<p>Given a road network and the locations of branches and the     headquarters in this network, your task is to determine the     minimum total distance that the couriers will need to travel to     deliver all the end-of-month messages, over all possible     assignments of branches to subprojects.</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The first line of input contains four integers      $n$,      $b$,      $s$, and      $r$, where      $n$ ($2     \le n \le 5\, 000$) is the number of intersections,     $b$ (     $1 \le b \le n-1$) is the number of     branches, $s$     ($1 \le s \le b$) is the     number of subprojects, and      $r$ ($1     \le r \le 50\, 000$) is the number of roads. The     intersections are numbered from      $1$ through      $n$. The branches are at intersections     $1$ through      $b$, and the headquarters is at     intersection $b + 1$. Each     of the next $r$ lines     contains three integers      $u$,      $v$, and      $\ell $, indicating a one-way road     from intersection $u$ to a     different intersection $v$     ($1 \leq u,v \leq n$) of     length $\ell $     ($0 \leq \ell \leq 10\,     000$). No ordered pair      $(u,v)$ appears more than once, and     from any intersection it is possible to reach every other     intersection.</p>
<h3>Output</h3>
<p>For each test case, display the minimum total distance that the couriers will     need to travel.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 4 2 10
5 2 1
2 5 1
3 5 5
4 5 0
1 5 1
2 3 1
3 2 5
2 4 5
2 1 1
3 4 2
5 4 2 10
5 2 1
2 5 1
3 5 5
4 5 10
1 5 1
2 3 1
3 2 5
2 4 5
2 1 1
3 4 2

<strong>Output:</strong>
13
24
    </pre>