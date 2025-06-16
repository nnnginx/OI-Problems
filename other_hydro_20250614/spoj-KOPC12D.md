<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are given the count of each digits and you have to create a number with these available digits.Let the number be X. In X each digit should not occupy any position which is divisible by the digit. 2 shouldn't occupy 2,4,6,8.. th positions and 7 shouldn't occupy 7,14th positions. Position of unit's place is 1, hundreds' place is 2. Suppose X =abcdef, f is in position 1 ,e is in position 2,d is in position 3, a is in position 6.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Now Find the length of smallest X as possible while filling the remaining postions with zeros.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Example: Count of 2=2,Count of 4 =2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">X can &nbsp;be &nbsp;40242,20442. But we need only the length of the number which is 5.</div>
<p>&nbsp;</p>
<p>You are given the count of each digits and you have to create a number with these available digits.Let the number be X. In X each digit should <strong>not</strong> occupy any position which is divisible by the digit. 2 shouldn't occupy 2,4,6,8.. th positions and 7 shouldn't occupy 7,14th positions. Position of unit's place is 1, hundreds' place is 2. Suppose X =abcdef, f is in position 1 ,e is in position 2,d is in position 3, a is in position 6.</p>
<p>Now Find the length of smallest X &nbsp;possible while filling the remaining postions with zeros.Minimize the length of the number generated.</p>
<p>Example: Count of 2=2,Count of 4 =2.</p>
<p>X can &nbsp;be &nbsp;40242, 20442. But we need only the length of the number which is 5.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input file contains T which denotes the number of test cases.This is followed by T lines where each of these T lines contains 8 space seperated integers which denotes the count of 2's , count of 3's,count of 4's .. upto count of 9's.</p>
<p>Note: Count of 1's will not be given as 1 divides every position of the number and Zeros can be placed in any position.</p>
<p>T&lt;=50,count of each digit&lt;=20.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>The output should contain T lines each line with the answer &nbsp;corresponding to a test case.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 0 2 0 0 0 0 0 
20 20 20 20 20 20 20 20


<strong>Output:</strong>
5
160

</pre>