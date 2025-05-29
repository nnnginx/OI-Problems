<h3>Binomial coefficients</h3>
<p>Gunnar is quite an old and forgetful researcher. Right now he is writing a paper on security in social networks and it actually involves some combinatorics. He wrote a program for calculating binomial coefficients to help him check some of his calculations.</p>
<p>A binomial coefficient is a number</p>
<img src="/NWERC11/content/problemA0x.png" alt="(n )        n!      =  ----------   k     k!(n - k)!  ">
<p>where <em>n </em>and <em>k </em>are non-negative integers.</p>
<p>Gunnar used his program to calculate <img src="/NWERC11/content/problemA1x.png" alt="(n)  k"> and got a number <em>m </em>as a result. Unfortunately, since he is forgetful, he forgot the numbers <em>n </em>and <em>k </em>he used as input. These two numbers were a result of a long calculation and they are written on one of many papers lying on his desk. Instead of trying to search for the papers, he tried to reconstruct the numbers <em>n,k </em>from the output he got. Can you help him and find all possible candidates? <!--l. 19--></p>
<h4>Input</h4>
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with an integer <em>m </em>(2 ¡Ü <em>m </em>¡Ü 10<sup>15</sup>): the output of Gunnar¡¯s program.</li>
</ul>
<h4>Output</h4>
<p>Per test case:</p>
<ul>
<li>one line with an integer: the number of ways of expressing <em>m </em>as a binomial coefficient. </li>
<li>one line with all pairs (<em>n,k</em>) that satisfy <img src="/NWERC11/content/problemA2x.png" alt="( )  n  k"> = <em>m</em>. Order them in increasing order of       <em>n </em>and, in case of a tie, order them in increasing order of <em>k</em>. Format them as in the       sample output.</li>
</ul>
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
<pre>2
2
15</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>1
(2,1)
4
(6,2) (6,4) (15,1) (15,14)</pre>
</td>
</tr>
</tbody>
</table>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>