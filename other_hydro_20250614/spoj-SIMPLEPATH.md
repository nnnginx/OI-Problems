<!-- 		@page { margin: 0.79in } 		p { margin-bottom: 0.1in; direction: ltr; color: #00000a; line-height: 120%; text-align: justify; orphans: 2; widows: 2 } 		p.western { font-family: "Calibri", serif; font-size: 11pt; so-language: en-US } 		p.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		p.ctl { font-family: ; font-size: 14pt; so-language: bn-BD } 	 -->
<p style="margin-bottom: 0.11in; line-height: 128%;" align="left"><span style="color: #000000;">You will be given a weighted rooted tree, where root is node 1. For each subtree of that tree, you will have to compute the summation of lengths of all possible simple paths present in that subtree. Eventually you need to print the summation of those values modulo </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>1000000007</strong></span></span><span style="color: #000000;">. </span></p>
<!-- 		@page { margin: 0.79in } 		p { margin-bottom: 0.1in; direction: ltr; color: #00000a; line-height: 120%; text-align: justify; orphans: 2; widows: 2 } 		p.western { font-family: "Calibri", serif; font-size: 11pt; so-language: en-US } 		p.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		p.ctl { font-family: ; font-size: 14pt; so-language: bn-BD } 	 -->
<p align="left"><span style="font-size: 11pt;">Image of the tree in the first sample is given below.</span></p>
<p style="text-align: center;" align="left"><span style="font-size: 11pt;"><img title="Tree in first sample" src="file://EmICN462.png" alt="Image of the tree in the first sample is given below." width="350" height="350"></span></p>
<p style="text-align: left;"><span style="font-size: 12pt;"><strong>Input Specification</strong></span></p>
<p style="margin-bottom: 0.14in; line-height: 115%;" align="left"><span style="color: #000000;">First line of input will contain an integer </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>T (1 &lt;= T &lt;= 10)</strong></span></span><span style="color: #000000;"> denoting the number of test cases. Each test case will begin with an integer </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>N (</strong></span></span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>1&lt;= N &lt;=100000</strong></span></span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>)</strong></span></span><span style="color: #000000;">, indicating number of nodes. The following </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>N-1</strong></span></span><span style="color: #000000;"> lines will have three integers each, </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>U (1 &lt;= U &lt;= N)</strong></span></span><span style="color: #000000;">, </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>V (1 &lt;= V &lt;= N)</strong></span></span><span style="color: #000000;">, </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>W (1 &lt;= W &lt;= 1000000000)</strong></span></span><span style="color: #000000;">, which denotes that there is an edge in the tree from node </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>U</strong></span></span><span style="color: #000000;"> to node </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>V</strong></span></span><span style="color: #000000;"> having </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>W</strong></span></span><span style="color: #000000;"> weight.</span></p>
<p style="margin-bottom: 0.14in; line-height: 115%;" align="left"><span style="color: #000000;"><span style="font-size: 11pt;"><strong>Input File is large. Use fast I/O methods.</strong></span></span></p>
<p style="margin-bottom: 0.14in; line-height: 115%;" align="left">&nbsp;</p>
<!-- 		@page { margin: 0.79in } 		h3 { margin-top: 0.14in; margin-bottom: 0in; direction: ltr; color: #4f81bd; line-height: 115%; text-align: justify; page-break-inside: avoid; orphans: 2; widows: 2 } 		h3.western { font-family: "Cambria", serif; font-size: 11pt; so-language: en-US } 		h3.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		h3.ctl { font-family: ; so-language: bn-BD } 		p { margin-bottom: 0.1in; direction: ltr; color: #00000a; line-height: 120%; text-align: justify; orphans: 2; widows: 2 } 		p.western { font-family: "Calibri", serif; font-size: 11pt; so-language: en-US } 		p.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		p.ctl { font-family: ; font-size: 14pt; so-language: bn-BD } 	 -->
<h3><span style="font-size: 12pt;">Output Specification</span></h3>
<p style="margin-bottom: 0.14in; line-height: 115%;" align="left"><span style="color: #000000;">For each test case, print the case number then print the answer to the problem modulo </span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>1000000007 </strong></span></span><span style="color: #000000;">in separate lines</span><span style="color: #000000;">.</span></p>
<!-- 		@page { margin: 0.79in } 		td p { margin-bottom: 0in; direction: ltr; color: #00000a; line-height: 100%; text-align: left; orphans: 0; widows: 0 } 		td p.western { font-family: "Liberation Serif", serif; font-size: 12pt; so-language: en-US } 		td p.cjk { font-family: "Droid Sans Fallback"; font-size: 12pt; so-language: zh-CN } 		td p.ctl { font-family: "FreeSans"; font-size: 12pt; so-language: hi-IN } 		p { margin-bottom: 0.1in; direction: ltr; color: #00000a; line-height: 120%; text-align: justify; orphans: 2; widows: 2 } 		p.western { font-family: "Calibri", serif; font-size: 11pt; so-language: en-US } 		p.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		p.ctl { font-family: ; font-size: 14pt; so-language: bn-BD } 	 -->
<h3><span style="font-size: 12pt;">Sample I/O</span></h3>
<table style="width: 639px;" border="0" cellspacing="0" cellpadding="2">
<colgroup><col width="314"> <col width="316"> </colgroup> 
<tbody>
<tr>
<td style="border: 1px solid #000001; padding-top: 0.02in; padding-bottom: 0.02in; padding-left: 0.06in; padding-right: 0.08in;" width="314" bgcolor="#ffffff">
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;"><strong>Sample 			Input</strong></span></span></span></p>
</td>
<td style="border: 1px solid #000001; padding-top: 0.02in; padding-bottom: 0.02in; padding-left: 0.06in; padding-right: 0.08in;" width="316" bgcolor="#ffffff">
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;"><strong>Sample 			Output</strong></span></span></span></p>
</td>
</tr>
<tr>
<td style="border: 1px solid #000001; padding-top: 0.02in; padding-bottom: 0.02in; padding-left: 0.06in; padding-right: 0.08in;" width="314" bgcolor="#ffffff">
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">2</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">7</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">1 			2 3</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">1 			3 2</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">2 			4 1</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">2 			5 4</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">3 			6 6</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">3 			7 8</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">6</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">1 			2 3</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">1 			3 2</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">1 			4 4</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">3 			5 7</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">3 			6 1</span></span></span></p>
</td>
<td style="border: 1px solid #000001; padding-top: 0.02in; padding-bottom: 0.02in; padding-left: 0.06in; padding-right: 0.08in;" width="316" bgcolor="#ffffff">
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">Case 			1: 212</span></span></span></p>
<p align="left"><span style="color: #000000;"><span style="font-family: Calibri, serif;"><span style="font-size: 11pt;">Case 			2: 109</span></span></span></p>
</td>
</tr>
</tbody>
</table>
<h3><span style="font-size: 12pt;">Explanation of Sample I/O</span></h3>
<!-- 		@page { margin: 0.79in } 		p { margin-bottom: 0.1in; direction: ltr; color: #00000a; line-height: 120%; text-align: justify; orphans: 2; widows: 2 } 		p.western { font-family: "Calibri", serif; font-size: 11pt; so-language: en-US } 		p.cjk { font-family: ; font-size: 11pt; so-language: en-US } 		p.ctl { font-family: ; font-size: 14pt; so-language: bn-BD } 	 -->
<p style="margin-bottom: 0.11in; line-height: 128%;" align="left"><span style="color: #000000;"><span style="font-size: 11pt;"><strong>Explanation of the 1st</strong></span></span><span style="color: #000000;"><span style="font-size: 11pt;"> </span></span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>sample:</strong></span></span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">Summation of lengths of all possible sample paths for each subtree is given below:<br> 1: 174</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">2: 10</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">3: 28</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">4: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">5: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">6: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">7: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 128%;" align="left"><span style="color: #000000;"><span style="font-size: 11pt;"><strong>Explanation of the 2</strong></span></span><span style="color: #000000;"><sup><span style="font-size: 11pt;"><strong>nd</strong></span></sup></span><span style="color: #000000;"><span style="font-size: 11pt;"> </span></span><span style="color: #000000;"><span style="font-size: 11pt;"><strong>sample:</strong></span></span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">Summation of lengths of all possible sample paths for each subtree is given below:</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">1: 93</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">2: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">3: 16</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">4: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">5: 0</span></p>
<p style="margin-bottom: 0.11in; line-height: 100%;" align="left"><span style="color: #000000;">6: 0</span></p>