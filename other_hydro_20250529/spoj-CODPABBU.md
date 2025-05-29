<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There is a biology experiment going in the biotech. lab of the "very prestigious" DTU.The students there are trying to study the reproduction patterns of a newly discovered species of virus pabbu-pneumoniae &nbsp; ;)&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">These pabbu-pneumoniae virus reproduce is a rather strange and fascinating way.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">After adding "a" number of viruses to the petri dish on the first day of they experiment they make the following observations</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">On the second day, they found that the virus' number had been increased by "d".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">On the third day, they found that the new number of viruses in the dish was "r" times the number recorded on the second day.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">On the fourth day, they again found that the number had increased by "d" by that recorded on the third day....and so on...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The pabbu-pneumoniae virus never ceases to reproduce.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For example, if d=1, r=4 and a = 1..then the number of microbes recorded on each day would be -:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2 8 9 36 37 148 149...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given 'a', 'd', 'r' and 'n', you have to find the number of microbes in the petri dish at the end of the n'th day...</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Since the numbers can be pretty large, you are required to print the answer modulo a number "m" ( "m" will be supplied for each case )</div>
<p>There is a biology experiment going in the biotech. lab of the "very prestigious" DTU.The students there are trying to study the reproduction patterns of a newly discovered species of virus pabbu-pneumoniae &nbsp; ;)&nbsp;</p>
<p>These pabbu-pneumoniae virus reproduce in a rather strange and fascinating way.</p>
<p>After adding "a" number of viruses to the petri dish on the first day of the experiment they make the following observations</p>
<p>On the second day, they found that the virus' number had been increased by "d".</p>
<p>On the third day, they found that the new number of viruses in the dish was "r" times the number recorded on the second day.</p>
<p>On the fourth day, they again found that the number had increased by "d" by that recorded on the third day....and so on...</p>
<p>The pabbu-pneumoniae virus never cease to reproduce.</p>
<p>For example, if d=1, r=4 and a = 1..then the number of microbes recorded on each day would be -:</p>
<p>1 2 8 9 36 37 148 149...</p>
<p>Given 'a', 'd', 'r' and 'n', you have to find the number of microbes in the petri dish at the end of the n'th day...</p>
<p>Since the numbers can be pretty large, you are required to print the answer modulo a number "m" ( "m" will be supplied for each case )</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>First line of input will have number 'T', the number of test cases. [ T &lt;= 2000 ]</p>
<p>Each of the test cases will have 2 lines -:</p>
<p>First line will have 3 space-separated numbers 'a' ,'d' &nbsp;and &nbsp; 'r' respectively.</p>
<p>2nd line will have 2 space-separated numbers 'n' &amp; 'm' respectively.</p>
<h3>Output</h3>
<p>For each test case print the required answer in a separate line.</p>
<p>NOTE - The value of a , d , r , n &amp; m will be more than 0 and less than 10^8.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1
1 2 3
4 5

<strong>Output:</strong>
1</pre>
<pre>EXPLANATION - The sequence is - 1,3,9,11,33,35,105.....
4th term is 11 and 11 % 5 = 1</pre>