<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Dr. Baws has an interesting problem. His $N$ graduate students, while friendly with some select people, are generally not friendly with each other. No graduate student is willing to sit beside a person they aren't friends with.</p>
<p><img src="../../../content/sourspinach:uoftcg.jpg" alt=""></p>
<p>The desks are up against the wall, in a single line, so it's possible that Dr. Baws will have to leave some desks empty. He does know which students are friends, and fortunately the list is not so long: it turns out that for any subset of $K$ graduate students, there are at most $K-1$ pairs of friends. Dr. Baws would like you to minimize the total number of desks required. What is this minimum number?</p>
<h3>Input</h3>
<p>The input begins with an integer $T \le 50$, the number of test cases. Each test case begins with two integers on their own line: $N \le 100000$, the number of graduate students (who are indexed by the integers $1$ through $N$), and $M$, the number of friendships among the students. Following this are $M$ lines, each containing two integers $i$ and $j$ separated by a single space. Two integers $i$ and $j$ represent a mutual friendship between students $i$ and $j$.</p>
<p>The total size of the input file does not exceed 2 MB.</p>
<h3>Output</h3>
<p>For each test case output a single number: the minimum number of desks Dr. Baws requires to seat the students.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">1<br>6 5<br>1 2<br>1 3<br>1 4<br>4 5<br>4 6</span></pre>
<pre><strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">7</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>As seen in the diagram, you seat the students in two groups of three with one empty desk in the middle.</p>