<p>Recently <a href="../JZPCIR/" target="_blank">Zippy</a> recieved four stacks, named A B C D respectively. Firstly, there are n elements in stack A (the element sequence is a permutation of 1..n), and stack B C D are empty. He can do four types of operations:</p>
<p>operation a: push the top element of stack A to stack B (if stack A is not empty, this operation can be done)</p>
<p>operation b: push the top element of stack B to stack D (if stack B is not empty, this operation can be done)</p>
<p>operation c: push the top element of stack A to stack C (if stack A is not empty, this operation can be done)</p>
<p>operation d: push the top element of stack C to stack D (if stack C is not empty, this operation can be done)</p>
<p>He can do 2*n operations in total. Obviously, there are n elements in stack D after he did the 2*n operations. Then he take out the top element in stack D one by one. If the first element he takes out is n, the second is n-1, ... , the last is 1, he will be very happy. Also, he wants to make the operation sequence he did lexicographic smallest.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line is a number t, which is the number of testcases.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The following t lines, each line contains a integer n, which is the number of sectors. (5&lt;=n&lt;=10^18)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Then following t testcases. For each test case, the first line contains a number n, which denotes the number of the elements in stack A. The second line contains n numbers, separated by a space, which are the elements in stack A, from top to the bottom.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each case, output a line. If there exists an answer, output the lexicographic smallest one. If not, output 0.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Example</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 3 4 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3 4 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">a b a c a b b d</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0Zippy jumps for years, and finally knows that jump is very boring. Then he found out a new way to&nbsp;</div>
<h3>Input</h3>
<p>First line is a number t, which is the number of testcases.&nbsp;</p>
<p>Then following t testcases. For each test case, the first line contains a number n, which denotes the number of the elements in stack A. The second line contains n numbers, separated by a space, which are the elements in stack A, from top to the bottom.</p>
<p>You can be sure that the sum of all n does not exceed 200000, and each n is not bigger than 100000.</p>
<h3><strong>Output</strong></h3>
<p>For each case, output a line. If there exists an answer, output the lexicographic smallest one (the operations Zippy does, separated by a space). If not, output 0.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>4<br>1 3 4 2<br>4<br>2 3 4 1<br><br><strong>Output:</strong><br>a b a c a b b d<br>0</pre>
<p><strong>Previous testdata wrong. All submissions have been rejudged. Sorry for inconvenience. &nbsp; (2011.10.5)</strong></p>