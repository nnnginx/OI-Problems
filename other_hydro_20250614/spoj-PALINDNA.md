<p>A DNA sequence is composed of a series of four possible nucleobases, namely Adenine, Guanine, Thymine and Cytosine; we will refer to each of these bases by their initial. For our purposes, nucleobases have an associated cyclic “order”: <tt>A</tt> is followed by <tt>G</tt>, which in turn is followed by <tt>T</tt>, which is followed by <tt>C</tt>, which is followed by <tt>A</tt> again. State-of-the-art research in genomics has revealed the startling fact that many diseases are caused by certain subsequences of bases not forming a palindromic sequence! Your mission as a leading researcher at ICPC laboratories is to take a DNA string <em>S</em> and a series of subsets <em>P</em><sub>1</sub>, …, <em>P</em><sub><em>t</em></sub> of indices to characters (nucleobases) in <em>S</em>, and transform <em>S</em> so that each of the restrictions of the resulting string to <em>P</em><sub>1</sub>, …, <em>P</em><sub><em>t</em></sub> are palindromic. (The restriction of <em>S</em> to a subset <em>P</em>={<em>i</em><sub>1</sub>, <em>i</em><sub>2</sub>, …, <em>i</em><sub><em>k</em></sub>} of indices, where 0 ≤ <em>i</em><sub>1</sub> &lt; <em>i</em><sub>2</sub> &lt; … &lt; <em>i</em><sub><em>k</em></sub> &lt; |<em>S</em>|, is the string <em>S</em><sub><em>i</em><sub>1</sub></sub> <em>S</em><sub><em>i</em><sub>2</sub></sub> … <em>S</em><sub><em>i</em><sub><em>k</em></sub></sub>). It is possible to inspect any base of <em>S</em> at will, but only three transformations can be applied to a base:</p>
<ol class="enumerate" type="1">
<li class="li-enumerate"> Leave it unaltered. </li>
<li class="li-enumerate">Increase it by 1 in the cyclic order of nucleobases (e.g. turn <tt>C</tt> into <tt>A</tt>). </li>
<li class="li-enumerate">Decrease it by 1 (e.g. turn <tt>T</tt> into <tt>G</tt>). </li>
</ol>
<p>Moreover, owing to limitations of current technology, it is impossible to modify two bases in consecutive positions of the sequence. Is our goal achievable?</p>
<p>By way of example, consider DNA sequence <tt>AGTAT</tt>. Number positions starting from 0, and suppose we have the three subsets <em>P</em><sub>1</sub> = {1, 4}, <em>P</em><sub>2</sub> = {0, 1} and <em>P</em><sub>3</sub> = {0, 2, 4}. One solution is to increase the first character and decrease the last, yielding <em>S</em>′ = <tt>GGTAG</tt>. The restrictions of <em>S</em>′ to <em>P</em><sub>1</sub>, <em>P</em><sub>2</sub> and <em>P</em><sub>3</sub> are <tt>GG</tt>, <tt>GG</tt> and <tt>GTG</tt>, respectively; all of them are palindromic.</p>
<p>One case where no solution is possible is when the string is <tt>CATGC</tt>, and we require the subsequences determined by positions {0,3} and {3,4} be palindromic. Here, characters 3, 0 and 4 would all need to become a <tt>T</tt>. But this entails modifying consecutive characters 3 and 4, which is not allowed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>The first line of each test case has two integers <em>N</em> and <em>T</em> (1 ≤ <em>N</em> ≤ 10&nbsp;000, 1 ≤ <em>T</em> ≤ 6&nbsp;000), the sequence length and number of subsets to consider. The next line contains the DNA sequence of length <em>N</em>, all of whose characters are in <tt>ACGT</tt>. The subsets are described by the following <em>T</em> lines. Each line starts by “<em>L</em>:”, where <em>L</em> (0 ≤ <em>L</em> ≤ <em>N</em>) is the number of positions in the subset, and is followed by <em>T</em> distinct integers between 0 and <em>N</em> − 1 in increasing order. Subsets may overlap partially or totally.</p>
<p>A blank line separates different test cases. The input file is terminated by a line containing <tt>0 0</tt>.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>In a single line per test case, print <tt>YES</tt> if the task is solvable and <tt>NO</tt> otherwise.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">5 3
AGTAT
2: 1 4
2: 0 1
3: 0 2 4

5 3
CATGC
0:
2: 0 3
2: 3 4

0 0
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">YES
NO
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: David García Soriano</em></blockquote>