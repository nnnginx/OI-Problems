<h3>  Bird tree</h3>
<!--l. 3-->
<p>The Bird tree<a id="fn1x0-bk" href="#fn1x0"><sup>1</sup></a> is an infinite binary tree, whose first 5 levels look as follows:</p>
<img src="/NWERC11/content/problemB0x.png" alt="                                   1                                    決1                     1決2                                  2決1          2決3                1決3                3決1                3決2    3        3         1        2        5         4        4        5    決5       決4       決4       決5        決2       決1       決3        決3 5   4    4    5   2    1    3   3    8    7   5    7   7    5    7   8 決8   決7   決5  決7   決7   決5  決7   決8  決3   決3   決1  決2   決5   決4  決4   決5 "> <!--l. 53-->
<p><!--l. 55--></p>
<p>It can be defined as follows:</p>
<img src="/NWERC11/content/problemB1x.png" alt="bird =             1決1          1決 (bird + 1)  (1決bird) + 1 "> <!--l. 60-->
<p>This is a <em>co-recursive </em>definition in which both occurrences of <em>bird </em>refer to the full (infinite) tree. The expression <em>bird </em>+ 1 means that 1 is added to every fraction in the tree, and 1<em>決bird </em>means that every fraction in the tree is inverted (so <sup><em>a</em></sup><em>決</em><sub><em>b</em></sub> becomes <sup><em>b</em></sup><em>決</em><sub><em>a</em></sub>). <!--l. 67--></p>
<p>Surprisingly, the tree contains every positive rational number exactly once, so every reduced fraction is at a unique place in the tree. Hence, we can also describe a rational number by giving directions (<tt>L</tt> for left subtree, <tt>R</tt> for right subtree) in the Bird tree. For example, <sup>2</sup><em>決</em><sub>5</sub> is represented by <tt>LRR</tt>. Given a reduced fraction, return a string  consisting of <tt>L</tt>＊s and <tt>R</tt>＊s: the directions to locate this fraction from the top of the tree. <!--l. 76--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 77-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with two integers <em>a </em>and <em>b </em>(1  ≒ <em>a,b </em>≒ 10<sup>9</sup>), separated by a <tt>＊/＊</tt>. These       represent the numerator and denominator of a reduced fraction. The integers <em>a </em>and       <em>b </em>are not both equal to 1, and they satisfy gcd(<em>a,b</em>) = 1.</li>
</ul>
<!--l. 87-->
<p>For every test case the length of the string with directions will be at most 10<span style="margin-left:0.3em">&nbsp;</span>000. <!--l. 90--></p>
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 91-->
<p>Per test case:</p>
<ul>
<li>one line with the string representation of the location of this fraction in the Bird tree.</li>
</ul>
<!--l. 97-->
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>3
1/2
2/5
7/3</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 107-->
<pre>L
LRR
RLLR</pre>
</td>
</tr>
</tbody>
</table>
<hr>
<p><a id="fn1x0" href="#fn1x0-bk"><sup>1</sup></a>Hinze, R. (2009). The Bird tree. J. Funct. Program., 19:491每508.</p>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>