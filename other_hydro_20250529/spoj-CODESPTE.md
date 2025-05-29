<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The country of Byteland contains of N cities and N - 1 bidirectional roads between them such that there a path between any two cities. The cities are numbered 0,...,N - 1. The people were very unhappy about the time it took to commute, especially salesmen who had to go about every city selling goods. So it was decided that new roads would be built. A new road was built between every two cities which could be reached from each other by travelling on exactly two old roads.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Now a salesman situated in city 0, just like any other typical salesman, has to visit all cities exactly once and return back to city 0 in the end. In how many ways can he do this?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains the number of test cases T. T test cases follow. The first line contains N, the number of cities in Byteland. The following N - 1 lines contain the description of the roads. The ith line contains two integers a_i and b_i, meaning that there was originally a road connecting cities with numbers a_i and b_i.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output T lines, one corresponding to each test case containing the required answer for that test case. Since the answers can be huge, output them modulo 1000000007.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 20</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= N &lt;= 10000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= a_i,b_i &lt; N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Explanation: For the first case, a new road was build between cities 0 and 2. Now, the salesman has two tour possibilities: 0-1-2-0 or 0-2-1-0.</div>
<p>&nbsp;</p>
<p>The country of Byteland contains of N cities and N - 1 bidirectional roads between them such that there a path between any two cities. The cities are numbered 0,...,N - 1. The people were very unhappy about the time it took to commute, especially salesmen who had to go about every city selling goods. So it was decided that new roads would be built. A new road was built between every two cities which could be reached from each other by travelling on exactly two old roads.</p>
<p>Now a salesman situated in city 0, just like any other typical salesman, has to visit all cities exactly once and return back to city 0 in the end. In how many ways can he do this?</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. T test cases follow. The first line contains N, the number of cities in Byteland. The following N - 1 lines contain the description of the roads. The ith line contains two integers a_i and b_i, meaning that there was originally a road connecting cities with numbers a_i and b_i.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines, one corresponding to each test case containing the required answer for that test case. Since the answers can be huge, output them modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 20</p>
<p>1 &lt;= N &lt;= 10000</p>
<p>0 &lt;= a_i,b_i &lt; N</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3</p>
<p>0 1</p>
<p>1 2</p>
<p>5</p>
<p>0 1</p>
<p>1 2</p>
<p>2 3</p>
<p>2 4</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2</p>
<p>4</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong> For the first case, a new road was build between cities 0 and 2. Now, the salesman has two tour possibilities: 0-1-2-0 or 0-2-1-0.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>