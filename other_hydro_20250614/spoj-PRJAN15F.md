<!-- h1 { margin-top: 0.14in; margin-bottom: 0in; direction: ltr; text-align: left; page-break-inside: avoid; widows: 2; orphans: 2; }h1.western { font-family: "Trebuchet MS",serif; font-size: 16pt; font-weight: normal; }h1.cjk { font-family: "Trebuchet MS"; font-size: 16pt; font-weight: normal; }h1.ctl { font-family: "Trebuchet MS"; font-size: 10pt; font-weight: normal; }p { margin-bottom: 0.1in; direction: ltr; line-height: 120%; text-align: left; widows: 2; orphans: 2; }a:link {  } -->
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Stack is a basic data structure. Where 3 operation can be done-</span></span></span></p>
<ol>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Push: 	You can push object to the stack</span></span></span></p>
</li>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Pop: 	You can pop the object to the stack</span></span></span></p>
</li>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Top: 	You can check the value of the top object.</span></span></span></p>
</li>
</ol>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">For further details you can get idea here ( if you really don��t know ) : <a href="https://en.wikibooks.org/wiki/Data_Structures/Stacks_and_Queues"><span style="color: #1155cc;"><span style="text-decoration: underline;">https://en.wikibooks.org/wiki/Data_Structures/Stacks_and_Queues</span></span></a></span></span></span></p>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></span></p>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Now we have a problem here, there are N stack in front of you. they are numbered from 1 to N. Each of them are initially empty. Now you will have Q operations. Each operation can be one the below 4 types:</span></span></span></p>
<ol>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">push 	i x, Push a value of x to stack numbered i</span></span></span></p>
</li>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">pop 	i, Pop value from the stack numbered i, if stack is empty discard 	the operation</span></span></span></p>
</li>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><a name="_GoBack"></a> put i j, Put the <strong>j��th </strong>stack on top of the <strong>i��th</strong> stack. So there will be no element left on the j��th stack.</span></span></span></p>
</li>
<li>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 	i, Print the value of the top element of ith stack. If stack is 	empty print ��Empty!��</span></span></span></p>
</li>
</ol>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></span></p>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Check the Sample IO for further understanding��</span></span></span></p>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br></span></span></span></p>
<p style="margin-bottom: 0in; line-height: 115%;"><span style="font-family: Calibri,serif;"><strong><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Input:</span></span></span></strong></span></p>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Input starts with an integer <strong>T (��5)</strong>, denoting the number of test cases.</span></span></span></p>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">The first line of a case is a blank line. The next line contains two integers <strong>N (1 �� N �� 10</strong><sup><strong>4</strong></sup><strong>)</strong>, <strong>Q(1 �� Q �� 5*10</strong><sup><strong>4</strong></sup><strong>)</strong>. </span></span></span></p>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">The next <strong>Q</strong> lines will contain a operation like above mentioned.</span></span></span></p>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><strong>(1</strong><strong>�� I, j �� N), (1�� x �� 10</strong><sup><strong>5</strong></sup><strong>)</strong></span></span></span></p>
<h1 style="margin-top: 0.33in;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><span style="color: #008000;"><strong><span style="color: #000000;">Output</span></strong></span></span></span></span></h1>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">For each test case, print the case number in a single line. Then for each 4th type operation you should print the value or ��Empty!�� if the stack is empty.</span></span></span></p>
<table style="width: 624px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="297"> <col width="297"> </colgroup> 
<tbody>
<tr valign="top">
<td style="border: 1.00pt solid #000001; padding: 0.07in;" width="297">
<p style="widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Input</span></span></span></p>
</td>
<td style="border: 1.00pt solid #000001; padding: 0.07in;" width="297">
<p style="widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Output</span></span></span></p>
</td>
</tr>
<tr valign="top">
<td style="border: 1.00pt solid #000001; padding: 0.07in;" width="297">
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">3 			18</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">push 			1 1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">push 			2 2</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">push 			3 3</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">push 			3 4</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			2</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			3</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">put 			1 3</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">pop 			2</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			2</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			3</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">pop 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">pop 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 			1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">pop 			1</span></span></span></p>
<p style="widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">top 1</span></span></span></p>
</td>
<td style="border: 1.00pt solid #000001; padding: 0.07in;" width="297">
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Case 			1:</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">2</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">4</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">4</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Empty!</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Empty!</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">3</span></span></span></p>
<p style="margin-bottom: 0in; widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">1</span></span></span></p>
<p style="widows: 0; orphans: 0;"><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Empty!</span></span></span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><strong><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;">Judge data is huge so use faster IO like scanf/printf</span></span></span></strong></p>
<p style="margin-bottom: 0.14in; line-height: 125%;" align="justify"><strong><span style="font-size: large;"><span style="font-size: small;"><span style="font-family: verdana, geneva;"><br>Problem-setter: Ahmad Faiyaz</span></span></span></strong></p>