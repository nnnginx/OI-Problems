<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2014 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a> ]</strong></p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Karina is developing a powerful encryption protocol. To make it available to a wider audience, she wants to implement a tool-kit to make it easier to use. In particular, she requires a tool capable of efficiently performing a complicated operation over strings.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The positions in a string are numbered from left to right with consecutive natural numbers from 1 to the length of the string. The operation Karina needs to implement is specified by 4 positions in the string i &lt;= j &lt; k &lt;= l, and consists of three steps:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1) interchange the substring that goes from position i to position j inclusive, with the substring that goes from position k to position l, inclusive;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2) reverse both substrings individually;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3) change all the characters of each substring into the next character in the alphabet. This is, every 'a' turns into a 'b', every 'b' turns into a 'c', etc. For the purposes of this operation we consider the alphabet to be circular, so that every 'z' turns into an 'a' after the operation is performed on it.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, let's take the string "alazareselfacil" and the positions i = 3, j = 5, k = 8 and l = 15, so that the two affected substrings are "aza" and "selfacil". After the first step (interchanging) the resulting string is "alselfacilreaza". After the second step (reversing) the result is "allicaflesreaza". Finally, after the third step (changing the characters to the ones following them) we obtain "almjdbgmftrebab".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The protocol developed by Karina applies the operation described above on a string, then applies another operation on the resulting string, and so on and so forth, always applying new operations on the last obtained result. Karina needs to know what is the resulting string after all operations are performed, but unfortunately her rudimentary knowledge of the programming language R is only enough to implement a very inefficient algorithm. You are therefore required to implement a version that can efficiently handle many operations over long strings.</div>
<p>Karina is developing a powerful encryption protocol. To make it available to a wider audience, she wants to implement a tool-kit to make it easier to use. In particular, she requires a tool capable of efficiently performing a complicated operation over strings.</p>
<p>The positions in a string are numbered from left to right with consecutive natural numbers from <strong>1</strong> to the length of the string. The operation Karina needs to implement is specified by four positions in the string <strong>i ��&nbsp;j &lt; k&nbsp;</strong><strong>��</strong><strong>&nbsp;l</strong>, and consists of three steps:</p>
<p>1) interchange the substring that goes from position <strong>i</strong> to position <strong>j</strong> inclusive, with the substring that goes from position <strong>k</strong> to position <strong>l</strong>, inclusive;</p>
<p>2) reverse both substrings individually;</p>
<p>3) change all the characters of each substring into the next character in the alphabet. This is, every <strong>'<span style="font-family: 'courier new', courier;">a</span>'</strong> turns into a <strong>'<span style="font-family: 'courier new', courier;">b</span>'</strong>, every <strong>'<span style="font-family: 'courier new', courier;">b</span>'</strong> turns into a <strong>'<span style="font-family: 'courier new', courier;">c</span>'</strong>, etc. For the purposes of this operation we consider the alphabet to be circular, so that every <strong>'<span style="font-family: 'courier new', courier;">z</span>'</strong> turns into an <strong>'<span style="font-family: 'courier new', courier;">a</span>'</strong> after the operation is performed on it.</p>
<p>For example, let's take the string "<span style="font-family: 'courier new', courier;">alazareselfacil</span>" and the positions <strong>i = 3, j = 5, k = 8</strong> and <strong>l = 15</strong>, so that the two affected substrings are "<span style="font-family: 'courier new', courier;">aza</span>" and "<span style="font-family: 'courier new', courier;">selfacil</span>". After the first step (interchanging) the resulting string is "<span style="font-family: 'courier new', courier;">al<strong>selfacil</strong>re<strong>aza</strong></span>". After the second step (reversing) the result is "<span style="font-family: 'courier new', courier;">al<strong>licafles</strong>re<strong>aza</strong></span>". Finally, after the third step (changing the characters to the ones following them) we obtain "<span style="font-family: 'courier new', courier;">al<strong>mjdbgmft</strong>re<strong>bab</strong></span>".</p>
<p>The protocol developed by Karina applies the operation described above on a string, then applies another operation on the resulting string, and so on and so forth, always applying new operations on the last obtained result. Karina needs to know what is the resulting string after all operations are performed, but unfortunately her rudimentary knowledge of the programming language R is only enough to implement a very inefficient algorithm. You are therefore required to implement a version that can efficiently handle many operations over long strings.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer number <strong>T</strong>, the number of test cases (<strong>1 �� T �� 100</strong>). <strong>T</strong> test cases follow.</p>
<p>The first line of each test case contains the initial string <strong>S</strong>, composed of between <strong>2</strong> and <strong>10<sup>5</sup></strong> lower-case letters of the English alphabet, and an integer <strong>N</strong>, representing the number of operations that are to be performed (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>5</sup></strong>).</p>
<p>The following <strong>N</strong> lines contain the description of one operation each, given by four integers <strong>I, J, K</strong> and <strong>L</strong> representing the four positions in the string for the operation explained above (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;I&nbsp;</strong><strong>��</strong><strong>&nbsp;J &lt; K&nbsp;</strong><strong>��</strong><strong>&nbsp;L&nbsp;</strong><strong>��</strong><strong>&nbsp;|S|</strong>&nbsp;with <strong>|S|</strong> the length of the string <strong>S</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing a string representing the resulting string obtained after succesively applying all the operations in the input to the given initial string.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
alazareselfacil 1
3 5 8 15
alazareselfacil 2
3 5 8 15
3 5 8 15
aa 1
1 1 2 2
zabcdefghi 5
1 1 10 10
1 5 6 10
2 4 7 9
1 1 2 10
1 8 9 10</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">almjdbgmftrebab
alcbcfsugnbgekn
bb
defghgjklm</span><span style="white-space: normal;">
</span></pre>