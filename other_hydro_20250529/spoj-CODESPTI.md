<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The country of Byteland contains of N cities and N - 1 bidirectional roads between them such that there a path between any two cities. The roads in Byteland were built long ago and now they are in need of repair. You have been hired to repair all the roads. You intend to do this by dispatching robots on some of the roads. Each robot will repair the road he is currently on and then move to one of the adjacent unrepaired roads. After repairing that, he will move to another adjacent unrepaired road, repair that and so on. Two roads are adjacent if they have the same city at one of their endpoints. For the process to be efficient, no two robots will can ever repair the same road, and no road can be visited twice. What is the least number of robots needed to accomplish the task?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow. The first line contains N, the number of cities in Byteland. The cities are numbered 0..N - 1. The following N - 1 lines contain the description of the roads. The ith line contains two integers a_i and b_i, meaning that there is a road connecting cities with numbers a_i and b_i.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one corresponding to each test case containing the required answer for that test case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 20</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= N &lt;= 10000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 &lt;= a_i,b_i &lt; N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">0 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Explanation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the first case, one robot is enough to repair all roads: (0,1) -&gt; (0,2) -&gt; (0,3)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the second case, one robot is again enough: (0,1) -&gt; (1,2) -&gt; (2,3) -&gt; (2,4) -&gt; (4,5)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The the third case, there is no way to repair all the roads with one robot and at least two are needed.</div>
<p>&nbsp;</p>
<p>The country of Byteland contains of N cities and N - 1 bidirectional roads between them such that there a path between any two cities. The roads in Byteland were built long ago and now they are in need of repair. You have been hired to repair all the roads. You intend to do this by dispatching robots on some of the roads. Each robot will repair the road he is currently on and then move to one of the adjacent unrepaired roads. After repairing that, he will move to another adjacent unrepaired road, repair that and so on. Two roads are adjacent if they have the same city at one of their endpoints. For the process to be efficient, no two robots will can ever repair the same road, and no road can be visited twice. What is the least number of robots needed to accomplish the task?</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. T test cases follow. The first line contains N, the number of cities in Byteland. The cities are numbered 0..N - 1. The following N - 1 lines contain the description of the roads. The ith line contains two integers a_i and b_i, meaning that there is a road connecting cities with numbers a_i and b_i.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines, one corresponding to each test case containing the required answer for that test case.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 20</p>
<p>1 &lt;= N &lt;= 10000</p>
<p>0 &lt;= a_i,b_i &lt; N</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3</p>
<p>4</p>
<p>0 1</p>
<p>0 2</p>
<p>0 3</p>
<p>6</p>
<p>0 1</p>
<p>1 2</p>
<p>2 3</p>
<p>2 4</p>
<p>4 5</p>
<p>7</p>
<p>0 1</p>
<p>1 2</p>
<p>2 3</p>
<p>2 4</p>
<p>4 5</p>
<p>3 6</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>1</p>
<p>1</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p>For the first case, one robot is enough to repair all roads: (0,1) -&gt; (0,2) -&gt; (0,3)</p>
<p>For the second case, one robot is again enough: (0,1) -&gt; (1,2) -&gt; (2,3) -&gt; (2,4) -&gt; (4,5)</p>
<p>The the third case, there is no way to repair all the roads with one robot and at least two are needed.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>