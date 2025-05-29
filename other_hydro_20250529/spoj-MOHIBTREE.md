<p>&nbsp;&nbsp;&nbsp;&nbsp;<strong><em> This Time Keyur(Singal) has been challenged by his friend  Nishant(Vaju).As keyur's programming skills are very poor so He asked  you to help him, So As a Great programmer you have to help keyur.The  challenge is as follow:<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Keyur has given a binary tree Mohib-tree. Every Mohib-tree has the following properties-<br>1. Every Mohib-tree contains a root node that stores a positive integer greater than or equal to 2.<br>2. Every node of an Mohib-tree is either a leaf node (has no children) or has exactly 2 children which are Mohib-trees as well.<br>The sum of values of children nodes is always equal to the value of the parent node.<br>Value of at least one of the children nodes divides the parent value.<br>The height of the tree is defined as the number of edges from the root to the deepest leaf.<br>Following is a valid Mohib-Tree:</em></strong></p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 6</strong></p>
<p>&nbsp;</p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp; /&nbsp;&nbsp; \&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; \</strong></p>
<p>&nbsp;</p>
<p><strong>&nbsp;&nbsp; 2&nbsp;&nbsp;&nbsp;&nbsp; 4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3</strong></p>
<p>&nbsp;</p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; /&nbsp; &nbsp;&nbsp; \</strong></p>
<p>&nbsp;</p>
<p><strong>&nbsp;&nbsp;&nbsp;&nbsp; 2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2</strong></p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-style: normal; font-variant: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><strong><em>Input Format :</em></strong></p>
<p>&nbsp;</p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 13px; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><strong><em>The first line of the input gives the number of test cases,<span>&nbsp;</span>T.<span>&nbsp;</span>T<span>&nbsp;</span>test cases follow. Each test case starts with one line with one integer<span>&nbsp;</span>N, which represents the value of the root node.</em></strong></p>
<p>&nbsp;</p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-style: normal; font-variant: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><strong><em>Output Format:</em></strong></p>
<p>&nbsp;</p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 13px; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><strong><em>For  each test case, output one line containing "Case #x:", where x is the  test case number (starting from 1). Then, for every value<span>&nbsp;</span>N<span>&nbsp;</span>in the test case, output the maximum possible height of all R-trees with root N.</em></strong></p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-style: normal; font-variant: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><em><strong>Constraints:</strong></em></p>
<p>&nbsp;</p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 13px; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><em><strong>0 &lt;<span>&nbsp;</span>T<span>&nbsp;</span>&lt;= 20</strong></em></p>
<p>&nbsp;</p>
<p style="color: #252c33; font-family: 'Open Sans', sans-serif; font-size: 13px; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: 18px; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; white-space: normal; widows: 1; word-spacing: 1px; -webkit-text-stroke-width: 0px; background-color: #ffffff;"><em><strong>2 &lt;=<span>&nbsp;</span>N<span>&nbsp;</span>&lt;= 10<sup>14</sup></strong></em></p>
<p>&nbsp;</p>
<p style="color: #000000; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: normal; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; widows: 1; word-spacing: 0px; -webkit-text-stroke-width: 0px; word-wrap: break-word; white-space: pre-wrap;"><em><strong>Input:</strong></em></p>
<p>&nbsp;</p>
<p><em><strong>3 </strong></em></p>
<p><em><strong>2</strong></em></p>
<p><em><strong> 6 </strong></em></p>
<p><em><strong>31</strong></em></p>
<p>&nbsp;</p>
<p><em><strong>Output:</strong></em></p>
<p>&nbsp;</p>
<pre style="color: #000000; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: normal; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; widows: 1; word-spacing: 0px; -webkit-text-stroke-width: 0px; word-wrap: break-word; white-space: pre-wrap;"><p style="color: #000000; font-style: normal; font-variant: normal; font-weight: normal; letter-spacing: normal; line-height: normal; orphans: auto; text-align: start; text-indent: 0px; text-transform: none; widows: 1; word-spacing: 0px; -webkit-text-stroke-width: 0px; word-wrap: break-word; white-space: pre-wrap;"><em><strong>Case #1: 0
Case #2: 2
Case #3: 0</strong></em></p><br></pre>