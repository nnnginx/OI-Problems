<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The mathematician Georg Cantor was a lover of both sets and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">infinity, but he didn't get along too well with his colleagues.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">One morning he woke up with the idea of defining a set so</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">strange that, when made public, would make the rest of the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">mathematicians lose their sleep for several days. And he was</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">successful.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The set he defined is called the Cantor set, and it is formed</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">by all the real numbers in the interval [0, 1] whose decimal</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">expression in base 3 uses exclusively the digits 0 and 2. This</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">set has amazing properties, which we will not mention here so</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">that you can sleep tonight. Moreover, and luckily for everyone</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">involved, in this problem we will not be working with the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Cantor set, but with a generalization of this set to the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">integer numbers.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We will say that an integer number is of Cantor type, or a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"cantiger" for short, if its expression in a given base B uses</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">solely the digits in a given set C contained in {0, 1, ...,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">B-1}. Thus, the fact that a given number is a cantiger depends</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">on how we choose B and C.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to count cantiger numbers, in order to prevent the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">mathematicians of the entire world from loosing their sleep.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">More precisely, given two integers D and H, along with B and C,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">you have to count the number of cantigers with respect to B and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">C from D to H inclusive.</div>
<p>The mathematician Georg Cantor was a lover of both sets and&nbsp;infinity, but he didn't get along too well with his colleagues.&nbsp;One morning he woke up with the idea of defining a set so&nbsp;strange that, when made public, would make the rest of the&nbsp;mathematicians lose their sleep for several days. And he was&nbsp;successful.</p>
<p>The set he defined is called the Cantor set, and it is formed&nbsp;by all the real numbers in the interval <strong>[0, 1]</strong> whose decimal&nbsp;expression in base <strong>3</strong> uses exclusively the digits <strong>0</strong> and <strong>2</strong>. This&nbsp;set has amazing properties, which we will not mention here so&nbsp;that you can sleep tonight. Moreover, and luckily for everyone&nbsp;involved, in this problem we will not be working with the&nbsp;Cantor set, but with a generalization of this set to the&nbsp;integer numbers.</p>
<p>We will say that an integer number is of Cantor type, or a&nbsp;<em>cantiger</em> for short, if its expression in a given base <strong>B</strong> uses&nbsp;solely the digits in a given set <strong>C</strong> contained in <strong>{0, 1, ...,&nbsp;B-1}</strong>. Thus, the fact that a given number is a cantiger depends&nbsp;on how we choose <strong>B</strong> and <strong>C</strong>.</p>
<p>Your task is to count cantiger numbers, in order to prevent the&nbsp;mathematicians of the entire world from loosing their sleep.&nbsp;More precisely, given two integers <strong>D</strong> and <strong>H</strong>, along with <strong>B</strong> and <strong>C</strong>,&nbsp;you have to count the number of cantigers with respect to <strong>B</strong> and&nbsp;<strong>C</strong> from <strong>D</strong> to <strong>H</strong> inclusive.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using a single line. This line&nbsp;contains three integers, <strong>D</strong>, <strong>H</strong> and <strong>B</strong>, and a string <strong>L</strong>. The values&nbsp;of <strong>D</strong> and <strong>H</strong> indicate the endpoints of the closed interval <strong>[D, H]</strong>&nbsp;we are interested in (<strong>1 ��&nbsp;D&nbsp;</strong><strong>��</strong><strong>&nbsp;H&nbsp;</strong><strong>��</strong><strong>&nbsp;10<sup>16</sup></strong>). The value of <strong>B</strong> is&nbsp;the base mentioned in the problem statement (<strong>2&nbsp;</strong><strong>��</strong><strong>&nbsp;B&nbsp;</strong><strong>��</strong><strong>&nbsp;10</strong>). The&nbsp;string <strong>L = L<sub>0</sub> L<sub>1</sub> ... L<sub>B-1</sub></strong> has exactly <strong>B</strong> characters, and&nbsp;describes the set <strong>C</strong> also mentioned in the problem statement.&nbsp;The character <strong>L<sub>i</sub></strong> is the uppercase letter <span style="font-family: 'courier new', courier;"><strong>'S'</strong></span> if <strong>i</strong> is in <strong>C</strong>, and&nbsp;the uppercase letter <span style="font-family: 'courier new', courier;"><strong>'N'</strong></span> otherwise (<strong>i = 0, 1, ..., B-1</strong>). The&nbsp;set <strong>C</strong> is non-empty, so that there is at least one <span style="font-family: 'courier new', courier;"><strong>'S'</strong></span> character&nbsp;in <strong>L</strong>. The end of the input is signalled by a line containing&nbsp;three times the number <strong>-1</strong> and a single <span style="font-family: 'courier new', courier;"><strong>'*'</strong></span> character.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing&nbsp;an integer number, representing the number of cantigers (with&nbsp;respect to <strong>B</strong> and <strong>C</strong>) that are greater or equal to <strong>D</strong> and lower or&nbsp;equal to <strong>H</strong>.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">1 10 3 SNS
99 999 5 NSSNS
1110 1111 10 NSNNNNNNNN
1 10000000000000000 10 NNNNNSNNNN
1 10000000000000000 7 SSSSSSS
-1 -1 -1 *</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">3
144
1
16
10000000000000000</span><span style="white-space: normal;">
</span></pre>