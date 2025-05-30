<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Advanced Ceiling Manufacturers (ACM) is analyzing the     properties of its new series of Incredibly Collapse-Proof     Ceilings (ICPCs). An ICPC consists of      $n$ layers of material, each with a     different value of collapse resistance (measured as a positive     integer). The analysis ACM wants to run will take the     collapse-resistance values of the layers, store them in a     binary search tree, and check whether the shape of this tree in     any way correlates with the quality of the whole construction.     Because, well, why should it not?</p>
<p>To be precise, ACM takes the collapse-resistance values for     the layers, ordered from the top layer to the bottom layer, and     inserts them one-by-one into a tree. The rules for inserting a     value $v$ are:</p>
<ul class="itemize">
<li>
<p>If the tree is empty, make          $v$ the root of the tree.</p>
</li>
<li>
<p>If the tree is not empty, compare          $v$ with the root of the tree. If         $v$ is smaller, insert         $v$ into the left         subtree of the root, otherwise insert          $v$ into the right subtree.</p>
</li>
</ul>
<p>ACM has a set of ceiling prototypes it wants to analyze by     trying to collapse them. It wants to take each group of ceiling     prototypes that have trees of the same shape and analyze them     together.</p>
<p>Given a set of prototypes, your task is to determine how     many different tree shapes they induce.</p>
<h3>Input</h3>
<p>Multiple test cases. Please process until EOF is reached. For each test case:</p>
<p>The first line contains two integers     $n$ (     $1 \le n \le 50$), which is the number     of ceiling prototypes to analyze, and      $k$ ($1     \le k \le 20$), which is the number of layers in each of     the prototypes.</p>
<p>The next $n$ lines     describe the ceiling prototypes. Each of these lines contains     $k$ distinct integers     (between $1$ and     $10^6$, inclusive), which     are the collapse-resistance values of the layers in a ceiling     prototype, ordered from top to bottom.</p>
<h3>Output</h3>
<p>For each test case, display the number of different tree shapes.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
5 3
2 7 1
3 1 4
1 5 9
2 6 5
9 7 3
3 4
3 1 2 40000
3 4 2 1
33 42 17 23

<strong>Output:</strong>
4
2

    </pre>