<p style="margin-bottom: 0in; line-height: 100%" align="CENTER"><span style="font-size: medium;"><strong>Guess the Queue</strong></span></p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">Busland is a city where the only means of transportation are buses. To get on a bus in Busland, people have to wait in queue. Each person has a <strong>unique</strong> bus <strong>ID</strong>. The person at the front is considered the first person and the person at the back is considered the last person in the queue. Trivially, the first person will get on the bus first and the last person will get on last.</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">It is well known that you should enter at the back of the queue. However, some people are very late and even though it is considered very rude, they try to enter in an alternative way. Since the sides of the queue are barricaded, the only alternative way is to enter from the front of the queue. Sometimes there are also people at the back of the queue, who become tired of waiting. They exit the queue from the back and just start walking to their destination instead.</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">Your task is to deal with three types of operations as follows:</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">1. ¡®<strong>1 </strong><em><strong>x y</strong></em>¡¯	The person with <strong>ID</strong><em><strong> y</strong></em> enters from the back or front, if <em><strong>x</strong></em> is ¡®<strong>B</strong>¡¯ or ¡®<strong>F</strong>¡¯ respectively.</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">2. ¡®<strong>2 </strong><em><strong>x¡¯</strong></em> The person in the back or front exits the queue, if <em><strong>x</strong></em> is ¡®<strong>B</strong>¡¯ or ¡®<strong>F</strong>¡¯ respectively.</p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-left: 1in; text-indent: -1in; margin-bottom: 0in; line-height: 100%" align="JUSTIFY">3. ¡®<strong>3 </strong><em><strong>x y¡¯</strong></em> Find the <strong>ID</strong> of the person in the <em><strong>y</strong></em>th position of the queue or the position of the queue, where the person with <strong>ID</strong> <em><strong>y</strong></em> is currently situated, if <em><strong>x</strong></em> is ¡®<strong>D</strong>¡¯ or ¡®<strong>P</strong>¡¯ respectively.</p>
<p style="margin-left: 1in; text-indent: -1in; margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><span style="font-size: small;"><strong>Input:</strong></span></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><a name="_GoBack"></a>The first line of input will contain the number of test cases, <em><strong>T</strong></em><strong> (1 &lt;= </strong><em><strong>T</strong></em><strong> &lt;= 5)</strong>. Then <em><strong>T </strong></em>cases follow.</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">Each case starts with an integer <em><strong>N</strong></em>, denoting the total number of operations. The following <em><strong>N</strong></em> lines will contain one of the three types described previously. The operations are in chronological order.<em><strong> </strong></em></p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">It is guaranteed that the given input is always valid. Thus, for the second type operation, the queue will always be non-empty and for the third type, the given position or <strong>ID </strong>will always exist in the queue. Also, a person who has already exited, will not enter the queue again.</p>
<p style="margin-bottom: 0in" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><span style="font-size: small;"><strong>Constraints:</strong></span><em><strong> </strong></em></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">For the <strong>easy</strong> version, <strong>1 &lt;= </strong><em><strong>N</strong></em><strong> &lt;= 2000</strong><em><strong> </strong></em></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">For the <strong>hard</strong> version, <strong>1 &lt;= </strong><em><strong>N</strong></em><strong> &lt;= 200000</strong></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">In general,</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><strong>1 &lt;= each ID &lt;= 10^9,</strong> IDs are <strong>unique</strong> for each person</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><strong>1 &lt;= each position &lt;= current size of the queue</strong></p>
<p style="margin-bottom: 0in; line-height: 100%" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><span style="font-size: small;"><strong>Output:</strong></span></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">For each case, print the case number on a single line, in the format ¡°<strong>Case x:</strong>¡±, where <em><strong>x </strong></em>is the case number.</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">For each operation of the third type, output a single integer, which denotes the answer of the query.</p>
<table style="width: 623px;" border="0" cellspacing="0" cellpadding="7">
<colgroup><col width="297"> <col width="297"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="297">
<p align="CENTER"><strong>Sample Input</strong></p>
</td>
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="297">
<p align="CENTER"><strong>Sample Output</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="297">
<p style="margin-bottom: 0in" align="JUSTIFY">1</p>
<p style="margin-bottom: 0in" align="JUSTIFY">7</p>
<p style="margin-bottom: 0in" align="JUSTIFY">1 B 1</p>
<p style="margin-bottom: 0in" align="JUSTIFY">1 B 2</p>
<p style="margin-bottom: 0in" align="JUSTIFY">1 F 3</p>
<p style="margin-bottom: 0in" align="JUSTIFY">3 D 3</p>
<p style="margin-bottom: 0in" align="JUSTIFY">2 B</p>
<p style="margin-bottom: 0in" align="JUSTIFY">1 F 4</p>
<p align="JUSTIFY">3 D 2</p>
</td>
<td style="border: 1px solid #00000a; padding-top: 0in; padding-bottom: 0in; padding-left: 0.08in; padding-right: 0.08in" width="297">
<p style="margin-bottom: 0in" align="JUSTIFY">Case 1:</p>
<p style="margin-bottom: 0in" align="JUSTIFY">2</p>
<p align="JUSTIFY">3</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><br><br></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><br><br></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY"><strong>Explanation of the Sample:</strong></p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">There is only 1 test case, in which we have to perform a total of 7 operations.</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">At first, the queue is empty. A person with <strong>ID 1 </strong>and <strong>2 </strong>enters from the back. After that, a person with <strong>ID 3 </strong>enters from the front. Now there are <strong>3</strong> people in the queue and the <strong>ID </strong>of the <strong>3</strong><sup><strong>rd</strong></sup><strong> </strong>person in the queue is <strong>2</strong>.</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">The person in the back (who has <strong>ID 2</strong>) exits the queue. This leaves only two people remaining.</p>
<p style="margin-bottom: 0.11in" align="JUSTIFY">Finally, a person with <strong>ID 4 </strong>enters from the front. Now there are again <strong>3</strong> people in the queue and the <strong>ID </strong>of the <strong>2</strong><sup><strong>nd</strong></sup> person of the queue is <strong>3</strong>.<br><span style="font-size: small;"><br><strong><span style="font-size: medium;">Problem Setter: Aninda Majumder</span></strong></span></p>