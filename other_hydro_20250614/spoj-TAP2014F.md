<p><strong>[ The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a> ]</strong></p>
<p>Strings are like plants in that they require a lot of loving care to grow. In this problem we will follow the evolution of a garden with <strong>N</strong> strings during a period covering <strong>T</strong> seasons. The strings in the garden are numbered from <strong>1</strong> to <strong>N</strong>, and are all initially empty. Each season we will perform two tasks in our garden:</p>
<p>- At the beginning of the season, we may <em>prune </em>the garden by deleting the <strong>C</strong> characters on the rightmost end of each of the <strong>N</strong> strings in the garden.</p>
<p>- After the pruning is done, we <em>fertilize </em>the garden so that each of the <strong>N</strong> strings grows by appending one character (possibly different for each string) to its rightmost end.</p>
<p>At the end of the season, a good string gardener always takes a moment to contemplate his/her work. In order to do this, we take a number <strong>P</strong> from <strong>1</strong> to <strong>N</strong> and then dedicate ourselves to appreciate the beauty of the string that stands at position <strong>P</strong> when we sort the <strong>N</strong> strings in the garden alphabetically from smallest to largest (breaking draws arbitrarily by putting first the strings identified with smaller numbers).</p>
<p>These moments of contemplation should be a well-deserved resting time for the gardener, so we don't want to waste time sorting the strings in the garden to identify the one we want to appreciate. Can you help us find it?</p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">period covering T seasons. The strings in the garden are numbered from 1 to N, and are all initially empty. Each season we will perform two tasks in our garden:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- At the beginning of the season, we may prune the garden by deleting the C characters on the rightmost end of each of the N strings in the garden.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">- After the prunning is done, we fertilize the garden so that each of the N strings grows by appending one character (possibly different for each string) to its rightmost end.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">At the end of the season, a good string gardener always takes a moment to contemplate his/her work. In order to do this, we take a number P from 1 to N and then dedicate ourselves to appreciate the beauty of the string that is at position P when we sort the N strings in the garden alphabetically from smallest to largest (breaking draws arbitrarily by putting first the strings identified with smaller numbers).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">These moments of contemplation should be a well-deserved resting time for the gardener, so we don't want to waste time sorting the strings in the graden to identify the one we want to appreciate. Can you help us find it?</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains two integer numbers <strong>N</strong> and <strong>T</strong>, representing the number of strings in the garden and the number of seasons we follow their evolution, respectively (<strong>2 ��&nbsp;N&nbsp;</strong><strong>��</strong><strong>&nbsp;100</strong>&nbsp;and <strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;T&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>4</sup></strong>). The following <strong>T</strong> lines describe one season each, in the same order in which they take place.</p>
<p>The description of each season consists of a number <strong>C</strong>, a string <strong>S</strong> and another number <strong>P</strong> (<strong>1&nbsp;</strong><strong>��</strong><strong>&nbsp;P&nbsp;</strong><strong>��</strong><strong>&nbsp;N</strong>). The number <strong>C</strong> is non-negative and represents the number of characters that are deleted during the pruning period at the beginning of the corresponding season (so it can be zero in case that no pruning is performed in that season). The string <strong>S</strong> contains exactly <strong>N</strong> characters <strong>s<sub>1</sub>, s<sub>2</sub>, ..., s<sub>N</sub></strong>, being the <strong>i</strong>-th character <strong>s<sub>i</sub></strong> the one that should be appended to the rightmost end of the string identified by the number <strong>i</strong> (<strong>s<sub>i</sub></strong> is a lower-case letter of the English alphabet for <strong>i = 1, 2, ..., N</strong>). Finally, the number <strong>P</strong> represents the position of the string we would like to appreciate at the end of the season, when we sort the <strong>N</strong> strings in the garden as explained in the problem statement.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print <strong>T</strong> lines, one for each season described in the input. The <strong>i</strong>-th line should contain the number identifying the string we want to appreciate at the end of the <strong>i</strong>-th season, for <strong>i = 1, 2, ..., T</strong>.</p>
<p>&nbsp;</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">2 4
0 aa 1
0 ba 1
1 ba 2
2 aa 2</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1
2
1
2</span></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">26 26
0 abcdefghijklmnopqrstuvwxyz 1
1 bcdefghijklmnopqrstuvwxyza 2
1 cdefghijklmnopqrstuvwxyzab 3
1 defghijklmnopqrstuvwxyzabc 4
1 efghijklmnopqrstuvwxyzabcd 5
1 fghijklmnopqrstuvwxyzabcde 6
1 ghijklmnopqrstuvwxyzabcdef 7
1 hijklmnopqrstuvwxyzabcdefg 8
1 ijklmnopqrstuvwxyzabcdefgh 9
1 jklmnopqrstuvwxyzabcdefghi 10
1 klmnopqrstuvwxyzabcdefghij 11
1 lmnopqrstuvwxyzabcdefghijk 12
1 mnopqrstuvwxyzabcdefghijkl 13
1 nopqrstuvwxyzabcdefghijklm 14
1 opqrstuvwxyzabcdefghijklmn 15
1 pqrstuvwxyzabcdefghijklmno 16
1 qrstuvwxyzabcdefghijklmnop 17
1 rstuvwxyzabcdefghijklmnopq 18
1 stuvwxyzabcdefghijklmnopqr 19
1 tuvwxyzabcdefghijklmnopqrs 20
1 uvwxyzabcdefghijklmnopqrst 21
1 vwxyzabcdefghijklmnopqrstu 22
1 wxyzabcdefghijklmnopqrstuv 23
1 xyzabcdefghijklmnopqrstuvw 24
1 yzabcdefghijklmnopqrstuvwx 25
1 zabcdefghijklmnopqrstuvwxy 26</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1
1</span><span style="white-space: normal;">
</span></pre>