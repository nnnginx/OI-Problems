<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Feeling sorry for all the mischief she has caused around the farm recently,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Bessie has agreed to help Farmer John stack up an incoming shipment of hay</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">bales. &nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">She starts with N (1 &lt;= N &lt;= 1,000,000, N odd) empty stacks, numbered 1..N.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">FJ then gives her a sequence of K instructions (1 &lt;= K &lt;= 25,000), each of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the form "A B", meaning that Bessie should add one new haybale to the top</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">of each stack in the range A..B. &nbsp;For example, if Bessie is told "10 13",</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">then she should add a haybale to each of the stacks 10, 11, 12, and 13.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">After Bessie finishes stacking haybales according to his instructions, FJ</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">would like to know the median height of his N stacks -- that is, the height</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">of the middle stack if the stacks were to be arranged in sorted order</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">(conveniently, N is odd, so this stack is unique). &nbsp;Please help Bessie</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">determine the answer to FJ's question.</div>
<p>&nbsp;</p>
<p>Feeling sorry for all the mischief she has caused around the farm recently,</p>
<p>Bessie has agreed to help Farmer John stack up an incoming shipment of hay</p>
<p>bales. &nbsp;</p>
<p>&nbsp;</p>
<p>She starts with N (1 &lt;= N &lt;= 1,000,000, N odd) empty stacks, numbered 1..N.</p>
<p>FJ then gives her a sequence of K instructions (1 &lt;= K &lt;= 25,000), each of</p>
<p>the form "A B", meaning that Bessie should add one new haybale to the top</p>
<p>of each stack in the range A..B. &nbsp;For example, if Bessie is told "10 13",</p>
<p>then she should add a haybale to each of the stacks 10, 11, 12, and 13.</p>
<p>&nbsp;</p>
<p>After Bessie finishes stacking haybales according to his instructions, FJ</p>
<p>would like to know the median height of his N stacks -- that is, the height</p>
<p>of the middle stack if the stacks were to be arranged in sorted order</p>
<p>(conveniently, N is odd, so this stack is unique). &nbsp;Please help Bessie</p>
<p>determine the answer to FJ's question.</p>
<p>INPUT</p>
<p>&nbsp;</p>
<p>* Line 1: Two space-separated integers, N K.</p>
<p>&nbsp;</p>
<p>* Lines 2..1+K: Each line contains one of FJ's instructions in the</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; form of two space-separated integers A B (1 &lt;= A &lt;= B &lt;= N).</p>
<p>&nbsp;</p>
<p>SAMPLE INPUT&nbsp;</p>
<p>7 4</p>
<p>5 5</p>
<p>2 4</p>
<p>4 6</p>
<p>3 5</p>
<p>&nbsp;</p>
<p>INPUT DETAILS:</p>
<p>&nbsp;</p>
<p>There are N=7 stacks, and FJ issues K=4 instructions. &nbsp;The first</p>
<p>instruction is to add a haybale to stack 5, the second is to add haybales</p>
<p>to stacks 2..4, etc.</p>
<p>&nbsp;</p>
<p>OUTPUT FORMAT:</p>
<p>&nbsp;</p>
<p>* Line 1: The median height of a stack after Bessie completes the</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; instructions.</p>
<p>&nbsp;</p>
<p>SAMPLE OUTPUT&nbsp;</p>
<p>1</p>
<p>&nbsp;</p>
<p>OUTPUT DETAILS:</p>
<p>&nbsp;</p>
<p>After Bessie is finished, the stacks have heights 0,1,2,3,3,1,0. &nbsp;The median</p>
<p>stack height is 1, since 1 is the middle element in the sorted ordering</p>
<p>0,0,1,1,2,3,3.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>