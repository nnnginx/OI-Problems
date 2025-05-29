<p><span id="docs-internal-guid-aca540d8-bd45-d1ed-dce2-0fd66a1300f8"> </span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Moumita doesn¡¯t like assignments. Whenever she is given any assignment, she feels helpless and wants to destroy the world. Unfortunately, she has a pending assignment. As she doesn¡¯t know how to do it, she is preparing to destroy everything. Can you help her to complete it and save the world???</span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><br></span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">The assignment is, you are given an array A of n elements and a function F(A) which is defined as:</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"> <img src="file://OWIkjb46.png" alt=""> </span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">where, <strong>mod = 2,760,727,302,517</strong></span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">You have to perform Q queries of the following types:</span></p>
<ol style="margin-top: 0pt; margin-bottom: 0pt;">
<li style="list-style-type: decimal; font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline;" dir="ltr">
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">1 x v &nbsp;( which means set A[x] = v. )</span></p>
</li>
<li style="list-style-type: decimal; font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline;" dir="ltr">
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">2 x v &nbsp;( which means add v to A[x] i.e., A[x] = A[x]+v. )</span></p>
</li>
<li style="list-style-type: decimal; font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;( which means compute F(A) and output it in a single line. )</span></li>
</ol>
<p>&nbsp;</p>
<h3>Input</h3>
<p><span id="docs-internal-guid-aca540d8-bd4f-9b81-ac5b-96a3147b1a01"> </span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Input starts with an integer </span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; font-weight: 700; vertical-align: baseline; white-space: pre-wrap;">T</span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"> denoting the number of test cases.</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">The first line of each case contains two integers </span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; font-weight: 700; vertical-align: baseline; white-space: pre-wrap;">n</span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"> and </span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; font-weight: 700; vertical-align: baseline; white-space: pre-wrap;">Q</span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">. The next line contains n space separated integers, where i</span><span style="font-size: 9.6px; font-family: Cambria; background-color: transparent; vertical-align: super; white-space: pre-wrap;">th</span><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"> integer denotes the value of A[i].</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Each of next Q lines contains a query of the above specified types.</span></p>
<h3><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">Constraints:</span></h3>
<p><span id="docs-internal-guid-aca540d8-bd51-22d7-39ba-20cc62b307ec"> </span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">1 ¡Ü T ¡Ü 6</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">1 ¡Ü x ¡Ü n ¡Ü 100000</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">1 ¡Ü Q ¡Ü 100000</span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; background-color: transparent; vertical-align: baseline; white-space: pre-wrap;">0 ¡Ü A[i], v ¡Ü 1000000000</span></p>
<h3>Output</h3>
<p><span id="docs-internal-guid-aca540d8-bd51-6a04-8cc2-ab3a4a2919e6"> </span></p>
<p style="line-height: 1.38; margin-top: 0pt; margin-bottom: 0pt; text-align: justify;" dir="ltr"><span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">For each case, print the case number first. Then for each query of &nbsp;type 3, print the value of F(A) in each line. See sample I/O for more clarification.</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span id="docs-internal-guid-aca540d8-bd51-a5fe-30cb-210fb82360c2">
<div style="margin-left: 0pt;" dir="ltr">
<table style="border: none; border-collapse: collapse; width: 624px;" border="0">
<colgroup><col width="*"><col width="*"></colgroup>
<tbody>
<tr style="height: 144px;">
<td style="vertical-align: top; padding: 7px 7px 7px 7px; border: solid #000000 1px;">
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">1</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">3 5</span><span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;"><br></span><span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">1 2 3</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">3</span><span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;"><br></span><span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">1 1 5</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">3</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">2 3 6</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">3</span>
</td>
</tr>
</tbody>
</table>
</div></span>
<strong>Output:</strong>
<span id="docs-internal-guid-aca540d8-bd51-d8bd-cd1f-f277eace363d">
<div style="margin-left: 0pt;" dir="ltr">
<table style="border: none; border-collapse: collapse; width: 624px;" border="0">
<colgroup><col width="*"><col width="*"></colgroup>
<tbody>
<tr style="height: 144px;">
<td style="vertical-align: top; padding: 7px 7px 7px 7px; border: solid #000000 1px;">
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">Case 1:</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">6</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">14</span>
<span style="font-size: 16px; font-family: Cambria; vertical-align: baseline; white-space: pre-wrap;">74</span></td>
</tr>
</tbody>
</table>
</div>
</span></pre>