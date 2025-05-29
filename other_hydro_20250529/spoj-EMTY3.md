<p>Let us introduce an algorithm with a function <strong>CanEmpty()</strong> which takes a string P as a parameter and return <strong>TRUE</strong> if it is possible to make P empty, otherwise return <strong>FALSE</strong>.</p>
<p>String P consists of only 0 and 1. The pseudo-code implementation of <strong>CanEmpty()</strong> function is as follows.</p>
<p>bool <strong>CanEmpty(</strong>String P<strong>)</strong></p>
<p>{</p>
<p>&nbsp;&nbsp;&nbsp; while(P has at least one substring 100)</p>
<p>&nbsp;&nbsp;&nbsp; {</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Chose any one substring 100 in P and delete it.</p>
<p>&nbsp;&nbsp;&nbsp; }</p>
<p>&nbsp;&nbsp;&nbsp; if(P is empty) return <strong>TRUE</strong>;</p>
<p>&nbsp;&nbsp;&nbsp; else return <strong>FALSE</strong>;</p>
<p>}</p>
<p>Now you are given a string S consisting of 0 and 1, you have to find the length of longest substring of <strong>S</strong> that can be made empty applying <strong>CanEmpty()</strong> algorithm.</p>
<p>As for example, let S=101<strong>110000</strong>0<strong>100</strong></p>
<p>S has only two sub-strings (bold) which can be made empty applying <strong>CanEmpty()</strong> algorithm.</p>
<p>The first substring will have the delete- sequence in <strong>CanEmpty() </strong>function :</p>
<p>1<span style="text-decoration: underline;">100</span>00-&gt;<span style="text-decoration: underline;">100</span>-&gt;empty</p>
<p>The second substring will have the delete-sequence in <strong>CanEmpty() </strong>function:</p>
<p><span style="text-decoration: underline;">100</span>-&gt;empty</p>
<p><strong>The length of first substring is 6 and second is 3. So, the required answer is 6.</strong></p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 100)</strong>, denoting the number of test cases.</p>
<p>Each case contains a string S. The size of string is at most <strong>200000</strong>.</p>
<p><strong>Output</strong></p>
<p>For each test case, print the case number and required answer.</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong>Sample   Input</strong></p>
</td>
<td width="319" valign="top">
<p><strong>Output   for Sample Input</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p>2<br> 1011100000100<br> 111011</p>
</td>
<td width="319" valign="top">
<p>Case 1:   6<br> Case 2: 0</p>
</td>
</tr>
</tbody>
</table>
<p><span style="font-family: Cambria, serif; font-size: 16px; font-style: italic; font-weight: bold; line-height: 18.4px;">Problem Setter: Md Abdul Alim, CEO and Founder at&nbsp;</span><a style="font-family: Cambria, serif; font-size: 16px; font-style: italic; font-weight: bold; line-height: 18.4px;" href="https://www.facebook.com/codemaskcp/">CodeMask</a></p>