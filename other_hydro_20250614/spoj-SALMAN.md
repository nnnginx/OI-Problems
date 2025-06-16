<p><strong><span style="font-family: verdana, geneva;">Salary Management</span></strong></p>
<p><span style="font-family: verdana, geneva;">You are working as a software engineer of Moogle! Now the boss of Moogle wants you to create a program which will efficiently handle some operations. At first, we should tell you about the structure of the employees at Moogle! Each employee has an integer id from 1 to N. Where 1 is the id of the Managing Director of Moogle! , who is the greatest boss of all the employees. Then except the Managing Director, each employee has an immediate boss. No employees have more than one immediate boss. Now your boss wants to have some operation like this �C</span></p>
<ol>
<li><span style="font-family: verdana, geneva;">He will give you an ID of an employee; you need to find the sum of salary of all the employees under that employee including him/herself.</span></li>
<li><span style="font-family: verdana, geneva;">He will give you an ID of an employee; you need to increase the salary of all the employees under that employee including him/herself by the minimum of minimum salary of all the employees under that employee including him/her and 1000.</span></li>
</ol>
<p><span style="font-family: verdana, geneva;">Let��s see the structure, hope you will get a clear idea about the problem.</span></p>
<p align="center"><span style="font-family: verdana, geneva;">&nbsp; <img src="file://39tmsnTd.png" alt="Employee Hiearchy" width="355" height="260"></span></p>
<p align="center"><span style="font-family: verdana, geneva;">Employee Hierarchy</span></p>
<p><span style="font-family: verdana, geneva;">Salary Table:</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="91" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">ID</span></p>
</td>
<td width="63" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">1</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">2</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">3</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">4</span></p>
</td>
<td width="76" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">5</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">6</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">7</span></p>
</td>
</tr>
<tr>
<td width="91" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">Salary (BDT)</span></p>
</td>
<td width="63" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">500</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">300</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">200</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">100</span></p>
</td>
<td width="76" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">10</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">200</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">100</span></p>
</td>
</tr>
</tbody>
</table>
<p align="center"><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;">Now if your boss wants to do the first operation for Employee ID 2. Then the output will be</span></p>
<p><span style="font-family: verdana, geneva;">300+100+200= 600 BDT</span></p>
<p><span style="font-family: verdana, geneva;">If your boss wants to do the second operation for the Employee ID 1, then the salary table becomes -</span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="91" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">ID</span></p>
</td>
<td width="63" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">1</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">2</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">3</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">4</span></p>
</td>
<td width="76" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">5</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">6</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">7</span></p>
</td>
</tr>
<tr>
<td width="91" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">Salary (BDT)</span></p>
</td>
<td width="63" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">510</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">310</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">210</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">110</span></p>
</td>
<td width="76" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">20</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">210</span></p>
</td>
<td width="77" valign="top">
<p align="center"><span style="font-family: verdana, geneva;">110</span></p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;">As minimum salary is 10 for Employee id 5 and which is less than 1000.</span></p>
<p><strong><span style="color: #339966;"><span style="font-family: verdana, geneva;">Input</span></span></strong></p>
<p><span style="font-family: verdana, geneva;">Input starts with an integer&nbsp;<strong>T (�� 3)</strong>, denoting the number of test cases.</span></p>
<p><span style="font-family: verdana, geneva;">The first line of a case is a blank line. The next line contains two integers&nbsp;<strong>N (1 �� N �� 10<sup>5</sup>)</strong>,&nbsp;<strong>q (1 �� q �� 50000)&nbsp;</strong>where&nbsp;<strong>N</strong>&nbsp;denotes the number of nodes and&nbsp;<strong>q</strong>&nbsp;denotes the number of queries. The nodes are numbered from&nbsp;<strong>1</strong>&nbsp;to&nbsp;<strong>N</strong>.</span></p>
<p><span style="font-family: verdana, geneva;">Then there will be&nbsp;<strong>N</strong>&nbsp;lines. The&nbsp;<strong>i<sup>th</sup>&nbsp;(1 �� i �� N)&nbsp;</strong>line contains two integers&nbsp;<strong>p<sub>i</sub></strong>&nbsp;and&nbsp;<strong>s<sub>i</sub></strong>&nbsp;<strong>(0 �� p<sub>i</sub>&nbsp;�� &nbsp;N, 1 �� s<sub>i</sub>&nbsp;&lt; 500)</strong>.&nbsp;<strong>p<sub>i</sub></strong>&nbsp;denotes the parent and&nbsp;<strong>s<sub>i</sub></strong>&nbsp;denotes the salary of the&nbsp;<strong>i<sup>th</sup></strong>&nbsp;employee, respectively. You can assume that the&nbsp;employee id with 1 is the managing director and only its parent is 0.</span></p>
<p><span style="font-family: verdana, geneva;">Each of the next&nbsp;<strong>q</strong>&nbsp;lines contains a query. Each query contains two integers:&nbsp;<strong>c</strong>&nbsp;and&nbsp;<strong>v (1 �� c �� 2, 1 �� v �� N)</strong>, where c denotes operation type, and v denotes the employee id. If the c = 1, then it means to do the first operation. If c=2, then the second operation.</span></p>
<p><span style="font-family: verdana, geneva;">You can assume that the input builds a valid rooted tree.</span></p>
<p><strong><span style="color: #339966;"><span style="font-family: verdana, geneva;">Output</span></span></strong></p>
<p><span style="font-family: verdana, geneva;">For each case, print the case number in a line. Then for each query type 1, print the sum of the salary.</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong><span style="color: #339966;"><span style="font-family: verdana, geneva;">Sample Input</span></span></strong></p>
</td>
<td width="319" valign="top">
<p><strong><span style="color: #339966;"><span style="font-family: verdana, geneva;">Output for Sample Input</span></span></strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p><span style="font-family: verdana, geneva;">1</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;">7 3</span></p>
<p><span style="font-family: verdana, geneva;">0 500</span></p>
<p><span style="font-family: verdana, geneva;">1 300</span></p>
<p><span style="font-family: verdana, geneva;">1 200</span></p>
<p><span style="font-family: verdana, geneva;">1 100</span></p>
<p><span style="font-family: verdana, geneva;">3 10</span></p>
<p><span style="font-family: verdana, geneva;">2 200</span></p>
<p><span style="font-family: verdana, geneva;">2 100</span></p>
<p><span style="font-family: verdana, geneva;">1 2</span></p>
<p><span style="font-family: verdana, geneva;">2 1</span></p>
<p><span style="font-family: verdana, geneva;">1 2</span></p>
</td>
<td width="319" valign="top">
<p><span style="font-family: verdana, geneva;">Case 1:</span></p>
<p><span style="font-family: verdana, geneva;">600</span></p>
<p><span style="font-family: verdana, geneva;">630</span></p>
</td>
</tr>
</tbody>
</table>
<p><strong><span style="font-family: verdana, geneva;">Note</span></strong></p>
<p><span style="font-family: verdana, geneva;">Dataset is huge. Use faster I/O methods.</span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p><span style="font-family: verdana, geneva;"><br></span></p>
<p>Problem Setter: Ahmad Faiyaz</p>
<p>Special Thanks: Syed Shahriar Manjur</p>