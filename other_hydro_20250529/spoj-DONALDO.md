<p style="margin-bottom: 0.14in; text-align: center"><span style="font-size: small;"><strong><span style="font-size: large;"><span style="font-family: "><span style="font-size: x-large;"><span style="font-family: ">Donaldo</span></span></span></span></strong></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: ">Donaldo is a great footballer. Since he is famous, he has lots of girlfriends. But the problem is, he isn't certain about the actual number of his girlfriends. So, he checked his mobile inbox. His girlfriends send him a lot of texts. But he knows that, none of them will send more than 1 text between <strong>I</strong> seconds of time interval. Given the exact times of received texts, Donaldo has to guess the minimum possible number of girlfriends he has.</span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: medium;"><strong><span style="font-size: small;"><span style="text-decoration: underline;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">Input</span></span></span></span></span></strong></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">The first line contains T(the number of test cases, <strong>0&lt;=T&lt;=50</strong>). Then T test cases follows.</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "><br></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">Each test case starts with a line with <strong>N</strong>(number of texts in Donaldo's inbox, <strong>0&lt;=N&lt;=20000</strong>). The following N lines contain a time of the format <strong>H:M:S</strong> (<strong>H</strong>=hour , <strong>M</strong>=minute, <strong>S</strong>=second, <strong>0&lt;=H&lt;=23</strong></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">,</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> <strong>0&lt;=M&lt;=59</strong>, <strong>0&lt;=S&lt;=59</strong>). The i-th time is the exact time when i-th text was received (<strong>1&lt;=i&lt;=N</strong>). The last line contains <strong>I</strong> (<strong>1&lt;=I&lt;=86400</strong>).</span></span></span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in"><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">Note that,</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "><br></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">1. A specific time can occur more than once.</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "><br></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">2. The texts are opened randomly, so the times don't have any particular(increasing/decreasing) order.</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "><br></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">3. The duration between sending and receiving a text is negligible.</span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: "><br></span></span></span></span><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">4. Intervals are inclusive. (e.g. If an interval of 5 seconds starts at 0:0:55, it will end at 0:0:59).</span></span></span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: medium;"><strong><span style="font-size: small;"><span style="text-decoration: underline;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">Output</span></span></span></span></span></strong></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "><span style="font-size: small;"><span style="font-family: "> </span></span></span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: "><span style="font-size: small;"><span style="font-family: ">For each testcase, output a line containing ��<strong>Case X: Y</strong>��, where X is the case number and Y is the minimum possible number of Donaldo's girlfriends.</span></span></span></span></p>
<table style="width: 639px;" border="0" cellspacing="0" cellpadding="7">
<colgroup> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0in" width="304">
<p align="JUSTIFY"><span style="font-size: medium;"><strong><span style="font-size: small;">Sample Input</span></strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0in 0.08in" width="305">
<p align="JUSTIFY"><span style="font-size: medium;"><strong><span style="font-size: small;">Output for Sample 			Input</span></strong></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0in" width="304">
<p align="JUSTIFY"><span style="font-size: small;"><strong>2</strong><br><strong>3</strong><br><strong>8:39:17</strong><br><strong>17:17:17</strong><br><strong>21:59:59</strong><br><strong>86400</strong><br><strong>3</strong><br><strong>17:17:17</strong><br><strong>21:59:59</strong><br><strong>8:39:16</strong><br><strong>48042</strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0in 0.08in" width="305">
<p style="margin-bottom: 0in"><span style="font-size: small;"><span style="color: #000000;"><strong>Case 			1: 3</strong></span><br><span style="color: #000000;"><strong>Case 			2: 2</strong></span></span></p>
<p>&nbsp;</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: medium;"><strong><span style="font-size: small;"><span style="text-decoration: underline;"><span style="font-family: ">Explanation</span></span></span></strong></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: ">In the first test, all the texts are inside 86400 seconds duration. That means, each text is sent by a distinct girlfriend. So, number of Donaldo's girlfriends has to be greater or equal to 3.</span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-size: small;"><span style="font-family: "> </span></span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p><span style="font-family: "> </span></p>
<p style="margin-bottom: 0.14in" align="JUSTIFY"><span style="font-size: small;"><span style="font-family: ">In the second case, there are 2 possible time intervals containing 2 texts. One is containing the 1st and the 3rd time, and the other is containing the 1st and the 2nd time. So, any answer smaller than 2 is not possible.</span></span></p>