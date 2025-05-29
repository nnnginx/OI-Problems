<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2015 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2015/09/pruebaTAP2015.pdf</a><span style="font-weight: bold;"> ]</span></p>
<p>There is a fundamental and unchanging characteristic shared by all life on Earth, from the tiniest microbe to whales, dinosaurs and human beings: DNA. This is the only known mechanism for the transmission and replication of genetic information, which poses one of the most important questions in modern biology: is DNA the only way to encode this information, or are there other possible mechanisms?</p>
<p>Professor Gould is a theoretical exobiologist whose research considers the possibility of the existence of extra-terrestrial life not having its genetic information encoded as DNA. Presently, he is developing a model based on the encoding of genetic information in the form of a chain of pseudo-nucleotides, which we will represent with the characters <strong>'<span style="font-family: 'courier new', courier;">b</span>', '<span style="font-family: 'courier new', courier;">d</span>', '<span style="font-family: 'courier new', courier;">o</span>', '<span style="font-family: 'courier new', courier;">p</span>', '<span style="font-family: 'courier new', courier;">q</span>', '<span style="font-family: 'courier new', courier;">v</span>', '<span style="font-family: 'courier new', courier;">w</span>'</strong> and <strong>'<span style="font-family: 'courier new', courier;">x</span>'</strong>. Each pseudo-nucleotide has a conjugate: <strong>'<span style="font-family: 'courier new', courier;">o</span>', '<span style="font-family: 'courier new', courier;">v</span>', '<span style="font-family: 'courier new', courier;">w</span>'</strong> and <strong>'<span style="font-family: 'courier new', courier;">x</span>'</strong> are each its own conjugate, whereas <strong>'<span style="font-family: 'courier new', courier;">b</span>'</strong> is the conjugate of <strong>'<span style="font-family: 'courier new', courier;">d</span>'</strong>, <strong>'<span style="font-family: 'courier new', courier;">p</span>'</strong> is the conjugate of <strong>'<span style="font-family: 'courier new', courier;">q</span>'</strong>, and conversely <strong>'<span style="font-family: 'courier new', courier;">d</span>'</strong> is the conjugate of <strong>'<span style="font-family: 'courier new', courier;">b</span>'</strong> and <strong>'<span style="font-family: 'courier new', courier;">q</span>'</strong> is the conjugate of <strong>'<span style="font-family: 'courier new', courier;">p</span>'</strong>.</p>
<p>In the model developed by professor Gould, an organism can suffer a mutation starting from a given position in its pseudo-nucleotide chain, resulting in the inversion and conjugation of the second part of said chain. Specifically, if the original pseudo-nucleotide chain is <strong>a<sub>1</sub>&nbsp;a<sub>2</sub>&nbsp;... a<sub>N</sub></strong>&nbsp;and the mutation occurs starting from position <strong>i</strong>, the resulting pseudo-nucleotide chain is <strong>a<sub>1</sub>&nbsp;a<sub>2</sub>&nbsp;... a<sub>i-1</sub>&nbsp;ã<sub>N</sub>&nbsp;ã<sub>N-1</sub>&nbsp;... ã<sub>i+1</sub>&nbsp;ã<sub>i</sub></strong>, where <strong>ã<sub>k</sub></strong>&nbsp;represents the conjugate of the pseudo-nucleotide originally at position <strong>k</strong>.</p>
<p>As it evolves, an organism may suffer many mutations in this manner, the only restriction being that successive mutations should occur starting from positions which are ever closer to the end of the pseudo-nucleotide chain. For example, the chain <strong>"<span style="font-family: 'courier new', courier;">bdopqvwx</span>"</strong> can suffer a mutation starting from position <strong>3</strong> resulting in the chain <strong>"<span style="font-family: 'courier new', courier;">bdxwvpqo</span>"</strong>, and after that another mutation starting from position &nbsp;<strong>7</strong> giving thus the chain <strong>"<span style="font-family: 'courier new', courier;">bdxwvpop</span>"</strong>, but these two mutations couldn't have occurred the other way around.</p>
<p>At this point in his research, professor Gould has two pseudo-nucleotide chains which are particularly interesting, and he would like to know the minimum number of mutations the first of them must suffer in order to become the second one. Can you help him?</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer <strong>N</strong>, representing the length of both pseudo-nucleotide chains to be analyzed (<strong>1 ≤ N ≤ 1000</strong>). Each of the following two lines contains a string of <strong>N</strong> characters&nbsp;<strong>'<span style="font-family: 'courier new', courier;">b</span>', '<span style="font-family: 'courier new', courier;">d</span>', '<span style="font-family: 'courier new', courier;">o</span>', '<span style="font-family: 'courier new', courier;">p</span>', '<span style="font-family: 'courier new', courier;">q</span>', '<span style="font-family: 'courier new', courier;">v</span>', '<span style="font-family: 'courier new', courier;">w</span>'</strong>&nbsp;and&nbsp;<strong>'<span style="font-family: 'courier new', courier;">x</span>'</strong>, representing a pseudo-nucleotide chain.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print one line containing an integer representing the minimum number of mutations the first chain in the input should suffer in order to become the second one. If this is not possible, print the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">8
bdopqvwx
bdxwvpop
5
bdopq
bdopq
10
ddbbddbbdd
bbddbbddbb
13
opoqpvbdxwwbp
vwpopvxxbdpqq</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">2
0
1
-1</span><span style="white-space: normal;">
</span></pre>