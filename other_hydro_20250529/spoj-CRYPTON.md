<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The young and very promising cryptogra-</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">pher Odd Even has implemented the security</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">module of a large system with thousands of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">users, which is now in use in his company.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The cryptographic keys are created from the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">product of two primes, and are believed to be</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">secure because there is no known method for</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">factoring such a product effectively.</div>
<p>&nbsp;</p>
<p>The young and very promising cryptographer Odd Even has implemented the security&nbsp;module of a large system with thousands of&nbsp;users, which is now in use in his company.&nbsp;The cryptographic keys are created from the&nbsp;product of two primes, and are believed to be&nbsp;secure because there is no known method for&nbsp;factoring such a product effectively.</p>
<div>
<div>What Odd Even did not think of, was that&nbsp;both factors in a key should be large, not just&nbsp;their product. It is now possible that some of&nbsp;the users of the system have weak keys. In a desperate attempt not to&nbsp;be fired, Odd Even secretly goes through all the users keys, to check if&nbsp;they are strong enough. He uses his very poweful Atari, and is especially&nbsp;careful when checking his boss�� key.</div>
</div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input consists of no more than 20 test cases. Each test case is a line&nbsp;with the integers 4 �� K �� 10^100 and 2 �� L �� 10^6 . K is the key itself, a&nbsp;product of two primes. L is the wanted minimum size of the factors in the&nbsp;key. The input set is terminated by a case where K = 0 and L = 0.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each number K, if one of its factors are strictly less than the required&nbsp;L, your program should output ��BAD p��, where p is the smallest factor in&nbsp;K. Otherwise, it should output ��GOOD��. Cases should be separated by a&nbsp;line-break.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
143 10
143 20
667 20
667 30
2573 30
2573 40
0 0

<strong>Output:</strong>
GOOD
BAD 11
GOOD
BAD 23
GOOD
BAD 31
</pre>