<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/MPART/en/">English</a></td> 
<td width="50%"><a href="/problems/MPART/vn/">Vietnamese</a></td> 
</tr></tbody></table>

<p>
Jamie is a very popular girl and has quite a lot of friends, so she always keeps a very long contact list in her cell phone. The lontact list has become so long that it often takes a long time for her to browse through the 
whole list to find a friend��s number.</p>
<p>
As Jamie��s best friend and a programming genius, you suggest that she group the contact list and minimize the size of the largest group, so that it will be easier for her to search for a friend��s number among the groups. Jamie takes your advice and gives you her entire contact list containing her friends�� names, the number of groups she wishes to have and what groups every friend could belong to.</p>
<p>Your task is to write a program that takes the list and organizes it into groups such that each friend appears in only one of those groups and the size
of the largest group is minimized. 
</p>
 
<h3>Input</h3>
<p>
There will be at most 20 test cases. Ease case starts with a line containing two integers N and M. where N is the length of the contact list and M is the number of groups. </p>
<p>N lines then follow. Each line contains a friend��s name and the groups the friend could belong to. You can assume N  is no more than 1000 and M is no more than 500. The names will contain alphabet letters only and will be no longer than 15 characters. No two friends have the
same name. The group label is an integer between 0 and M-1. </p>
<p>After the last test case, there is a single line ��0 0�� that terminates the input.  
</p>

<b>Sample Input</b>
<pre>3 2 
John 0 1 
Rose 1 
Mary 1 
5 4 
ACM 1 2 3 
ICPC 0 1  
Asian 0 2 3 
Regional 1 2 
ShangHai 0 2 
0 0 
</pre>

<h3>Output</h3>
<p> 
For each test case, output a line containing a single integer, the size of the largest contact group.
</p>

<b>Sample output</b>
<pre>2
2
</pre>
<b>Note : Huge data input </b>