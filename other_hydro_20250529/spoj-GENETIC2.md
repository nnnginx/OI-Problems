<p>A colony of alien bacteria has recently been discovered close to a crater in New Mexico. Dr. Poucher is in charge of the scientific team at the ICPC BioLab committed to the study of the alien DNA structure. We briefly sketch their discoveries here.</p>
<p>Alien DNA molecules have the structure of a circular sequence. Each sequence is composed of nucleotides. There are 26 different types of nucleotides, and each of them can occur in two faces. It is very important to remark that in any given alien DNA molecule, every nucleotide either does not appear at all or appears exactly twice (hence, the length of a DNA molecule is an even integer between 2 and 52). In case a nucleotide occurs twice, each occurrence can be of either type independently. Alien bacteria have two types of extremities, which in the technical biological jargon are referred to as arms and legs. A major discovery of Dr. Poucher’s team is a method to determine the exact number of arms and legs of a bacterium by examining its DNA structure.</p>
<p>Here we represent each nucleotide as a letter of the alphabet. We refer to the different nucleotides as <tt>a</tt>, <tt>A</tt>, …<tt>z</tt>, <tt>Z</tt>, where the lowercase and uppercase forms of a letter represent the two possible faces a nucleotide may appear with; we shall also use <em>a</em>/<em>A</em>, <em>b</em>/<em>B</em>, …<em>z</em>/<em>Z</em> to refer to a nucleotide in either face.</p>
<p>To determine the number of extremities, Dr. Poucher starts by initializing two counters of arms and legs to zero, and then proceeds to perform a number of surgeries, transforming a DNA sequence into another one. After each transformation, you may need to increase some of the counters, depending on the type of surgery applied. When the empty sequence of nucleotides (which will be denoted by ∅) has been reached, the number of extremities of the original molecule has been found. The possible surgeries are:</p>
<ol class="enumerate" type="1">
<li class="li-enumerate">Eliminate consecutive instances of a given nucleotide appearing with opposite faces. The number of arms and legs is preserved. For example: <tt>aBbCaC</tt> → <tt>aCaC</tt> by eliminating <tt>Bb</tt>. Another example: <tt>DeHhEd</tt>→ <tt>eHhE</tt> by eliminating <tt>dD</tt>. Remember that DNA structure is circular, so in our representation as a string the last and first letters are connected.</li>
<li class="li-enumerate">Eliminate consecutive nucleotides appearing with the same face. Add one to the number of arms. For example: <tt>BBcgCg</tt> → <tt>cgCg</tt> by eliminating <tt>BB</tt>. Another example: <tt>xabyyaBX</tt> → <tt>xabaBX</tt> by eliminating <tt>yy</tt>.</li>
<li class="li-enumerate">Eliminate a sequence of four nucleotides formed by two different nucleotides that appear alternately where different occurrences of the same nucleotide have opposite faces. Add one to the number of legs. For example: <tt>dcDCefFe</tt> → <tt>efFe</tt>, by eliminating <tt>dcDC</tt>. Another example: <tt>cmNMnC</tt> → <tt>cC</tt> by eliminating <tt>mNMn</tt>.</li>
<li class="li-enumerate">Cut and paste, the most sophisticated procedure. First, a nucleotide is selected, for instance <em>a</em>/<em>A</em>, and the DNA sequence is chopped into two linear chains such that the nucleotide appears once in each of them.
<p>Second, if both occurrences of <em>a</em>/<em>A</em> are of the same face, one of the chains is “inverted” by reversing the sequence and changing the face of every nucleotide in the chain. Given a chain <em>S</em>, <span style="text-decoration:overline">S</span> denotes its “inverted” chain.</p>
<p>Then, the chains are combined by concatenating the subsequence occurring before <tt>a</tt> with the subsequence occurring after <tt>A</tt>, and the subsequence occurring after <tt>a</tt> with the sub-sequence occurring before&nbsp;<tt>A</tt>.</p>
<p>Finally, two new <em>a</em>/<em>A</em> nucleotides are added to close the chain into a circular shape. The face of the new nucleotides are the same if the original pair of nucleotides selected had the same face, and is different otherwise.</p>
<p>Formally, suppose you select the nucleotide <em>a</em>/<em>A</em>, and further assume for the moment that it appears both times with the face <tt>a</tt> (<tt>A</tt>). The cut and paste surgery turns sequences of the form <em>S</em><sub>1</sub><tt>a</tt><em>S</em><sub>2</sub><em>S</em><sub>3</sub><tt>a</tt><em>S</em><sub>4</sub> (respectively <em>S</em><sub>1</sub><tt>A</tt><em>S</em><sub>2</sub><em>S</em><sub>3</sub><tt>A</tt><em>S</em><sub>4</sub>) into <em>S</em><sub>2</sub><tt>a</tt><em>S</em><sub>1</sub><span style="text-decoration:overline">S_3</span><tt>a</tt><span style="text-decoration:overline">S_4</span> (respectively <em>S</em><sub>2</sub><tt>A</tt><em>S</em><sub>1</sub><span style="text-decoration:overline">S_3</span><tt>A</tt><span style="text-decoration:overline">S_4</span>). On the other hand, if nucleotide <em>a</em>/<em>A</em> appears with its two different faces, the surgery turns sequences of the form <em>S</em><sub>1</sub><tt>a</tt><em>S</em><sub>2</sub><em>S</em><sub>3</sub><tt>A</tt><em>S</em><sub>4</sub> into <em>S</em><sub>2</sub><tt>a</tt><em>S</em><sub>1</sub><em>S</em><sub>4</sub><tt>A</tt><em>S</em><sub>3</sub>. <em>S</em><sub>1</sub>, <em>S</em><sub>2</sub>, <em>S</em><sub>3</sub> and <em>S</em><sub>4</sub> are arbitrary sub-chains (possibly empty). In both cases the original circular chain was chopped into <em>S</em><sub>1</sub>(<em>a</em>/<em>A</em>)<em>S</em><sub>2</sub> and <em>S</em><sub>3</sub>(<em>a</em>/<em>A</em>)<em>S</em><sub>4</sub>.</p>
<p>For example (see the figure below): starting with the sequence <tt>BacDcAbD</tt>, we can get chains <tt>BacDc</tt> and <tt>AbD</tt>. Then, merging at nucleotide <em>a</em>/<em>A</em> we get the sequence <tt>cDca’BbDA’</tt> where <tt>a’</tt> and <tt>A’</tt> represent the new <em>a</em>/<em>A</em> nucleotides. Here, <em>S</em><sub>1</sub> = <tt>B</tt>, <em>S</em><sub>2</sub> = <tt>cDc</tt>, <em>S</em><sub>3</sub> = ∅ and <em>S</em><sub>4</sub> = <tt>bD</tt>.</p>
<p>Another example: take the same DNA sequence <tt>BacDcAbD</tt>, and cut to get the chains <tt>DBac</tt> and <tt>DcAb</tt>; paste nucleotide <em>c</em>/<em>C</em> (in this case you need to reverse one chain, for example <tt>BaCd</tt>) to get the sequence <tt>cDBadcBa</tt>. Here, <em>S</em><sub>1</sub> = <tt>DBa</tt>, <em>S</em><sub>2</sub> = ∅, <em>S</em><sub>3</sub> = <tt>D</tt> and <em>S</em><sub>4</sub> = <tt>Ab</tt>.</p>
<blockquote class="figure">
<div class="center">
<hr size="2">
</div>
<div class="center"><img src="../../../content/elhipercubo:sequence.jpg" alt="">
<div class="caption">
<table border="0" cellspacing="6" cellpadding="0">
<tbody>
<tr>
<td align="left" valign="top">Figure 1: First example of use of cut&amp;paste</td>
</tr>
</tbody>
</table>
</div>
</div>
<div class="center">
<hr size="2">
</div>
</blockquote>
<p>This surgery does not modify the number of arms or legs, but can be used cleverly in combination with the previous surgeries to reduce the size of the DNA molecule and finish the calculation.</p>
</li>
</ol>
<p>However, alien bacteria do not present both arms and legs at the same time. This is due to the fact that, in their early development, a leg, in the presence of one or more arms, becomes two arms. Because of the above, the end result is either a number of arms or a number of legs, but not both at the same time. In order to avoid expensive surgical procedures, Dr. Poucher has hired you to write a program that computes the number of arms and legs a bacterium will develop, given its DNA sequence. It is guaranteed that the result is determined uniquely by the original string, regardless of the particular sequence of surgeries applied.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Input</span></span></strong></p>
<p>Each test case consists of a string of even length between 2 and 52, inclusive, representing the DNA structure of an alien bacterium. All characters are letters. There will be one case per line in the input. The last line contains the word “END” and must not be processed.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Output</span></span></strong></p>
<p>The output for each test case should have exactly one line, containing the number of arms or legs the bacterium will have, followed by the word “arms” or “legs” respectively (if the number is 1, the words should be in singular). In case there will be neither arms nor legs, the program should print the word “none”.</p>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Input</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">rkrk
abcdeABCDE
shcoOCfFHS
END
</pre>
</div>
<p><br> <br> <strong><span style="color: black;"><span style="font-size: medium;">Sample Output</span></span></strong></p>
<div class="minipage">
<pre class="verbatim">1 arm
2 legs
none
</pre>
</div>
<!--CUT END --> <!--HTMLFOOT--> <!--ENDHTML--> <!--FOOTER--> 
<hr size="2">
<blockquote class="quote"><em>Problemsetter: Luis Hernández Corbato</em></blockquote>