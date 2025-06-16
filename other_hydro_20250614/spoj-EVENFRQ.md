<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Kutus loves even number. Girl friend of kutus, name putus makes an interesting</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">problem for kutus to testing his even number knowledge. Putus gives an integer</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">array A, consisting of N number.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Putus asked Kutus to process the following three types of queries on this array</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">accurately and efficiently.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• 0 X V: add V to the Xth element of array. i.e AX = AX + V.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• 1 L R V: replace all the element in range L to R with V.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">• 2 L R: Find out whether all elements frequency in the range L to R is/are even or</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">not</div>
<p>Kutus loves even number. Girl friend of kutus, name putus makes an interesting problem for kutus to testing his even number knowledge. Putus gives an integer array A, consisting of N number.</p>
<p>Putus asked Kutus to process the following three types of queries on this array accurately and efficiently.</p>
<p>• 0 X V: add V to the Xth element of array. i.e AX = AX + V.</p>
<p>• 1 L R V: replace all the element in range L to R with V.</p>
<p>• 2 L R: Find out whether all elements frequency in the range L to R is/are even or not</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Input start with an integer T, which denotes the number of test case. Each case contains 2 space separated integer N and Q denoting the size of array A and the number of queries to be performed.</p>
<p>Next line contains N space separated integers denoting the elements of array A. Each of the next Q lines of input contains a query having one of the mentioned three types. There will be no more than fifty update operation (type 0 &amp; type 1).</p>
<h3>Output</h3>
<p>For each case print the case number and print the answer. If all elements frequency in the range L to R is/are even, then answer will be ‘Yes’ otherwise answer will be ‘No’.</p>
<p>&nbsp;</p>
<p><strong><span style="font-size: x-small;"><span style="font-size: small;">Constraints</span>:</span></strong></p>
<p>T &lt;= 10</p>
<p>1 &lt;= N &lt;= 100000</p>
<p>1 &lt;= Q &lt;= 100000</p>
<p>0 &lt;= Ai , V &lt;= 100000</p>
<p>1 &lt;= L &lt;= R &lt;= N</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; line-height: 20px;">1
5 6
1 2 2 3 2
2 2 3
0 5 1
2 2 5
2 1 5
1 1 3 2
2 1 5</span>

<strong>Output:</strong>
<span style="color: #3e3f3a; font-family: &quot;Ubuntu Mono&quot;; font-size: 14px; line-height: 20px;">Case 1:
Yes
Yes
No
No</span></pre>