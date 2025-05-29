<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The ancient civilization of the Prendonians, who lived in Jutland from 5000 BC to 4500</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">BC, is well known. A Prendonian name is composed of three non empty words formed by</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">lowercase letters from a to z: an unique ﬁrst name, one of their parents’ ﬁst name with a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">suﬃx and the other parent’s name with the same suﬃx. The unique ﬁrst name always comes</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">ﬁrst, but there is no speciﬁc order for the other two.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The suﬃx denotes the gender of the bearer of the name, jk for male and gvw for female,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">for example, if ric is igo and malte’s son, his full name would be ric igojk maltejk, but had</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">ric been a girl, his name would have been ric igogvw maltegvw.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">All the Prendonians were monogamic and faithful to their partners. There are no registers</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">of male homosexual couples, but it was common for two women to be married, and there has</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">not been a single case of married siblings in Prendonian history. A couple was not considered</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">married until they had given birth to a child or adopted one.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given N 3 word names, write a program that prints Y ES if they are all valid and part of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">a valid Prendonian family tree and everyone is related to everyone else, print N O otherwise.</div>
<p>&nbsp;</p>
<p>The ancient civilization of the Prendonians, who lived in Jutland from 5000 BC to 4500</p>
<p>BC, is well known. A Prendonian name is composed of three non empty words formed by</p>
<p>lowercase letters from a to z: an unique ﬁrst name, one of their parents’ ﬁst name with a</p>
<p>suﬃx and the other parent’s name with the same suﬃx. The unique ﬁrst name always comes</p>
<p>ﬁrst, but there is no speciﬁc order for the other two.</p>
<p>The suﬃx denotes the gender of the bearer of the name, jk for male and gvw for female,</p>
<p>for example, if ric is igo and malte’s son, his full name would be ric igojk maltejk, but had</p>
<p>ric been a girl, his name would have been ric igogvw maltegvw.</p>
<p>All the Prendonians were monogamic and faithful to their partners. There are no registers</p>
<p>of male homosexual couples, but it was common for two women to be married, and there has</p>
<p>not been a single case of married siblings in Prendonian history. A couple was not considered</p>
<p>married until they had given birth to a child or adopted one.</p>
<p>Given N 3 word names, write a program that prints Y ES if they are all valid and part of</p>
<p>a valid Prendonian family tree and everyone is related to everyone else, print N O otherwise.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The ﬁrst line consists of a single integer T (1 ≤ T ≤ 30), which is the number of test</p>
<p>cases. Each test case begins with a line with only the integer N (1 ≤ N ≤ 1000), the number</p>
<p>of names, followed by N lines with 3 word (a-z lowercase only, each word not longer than 103</p>
<p>characters), the ﬁrst word is garanteed to be unique.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case print YES if the names are all valid and part of a valid Prendonian</p>
<p>family tree and are all related to each other, print NO otherwise.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
3
docs afegvw fegvw
draw rridajk cajk
pito docsjk drawjk

<strong>Output:</strong>
YES</pre>