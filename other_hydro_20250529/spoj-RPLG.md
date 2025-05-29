<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;Vero is working on an important company, the company noticed that Vero codes using goto labels, her boss does not want Vero to code this kind of programs, the boss tells her that he will cut her payment by the number of lines contained between the label and the goto.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Vero does not know any iterative structures, and she is too worried to code the program she is asking you for, Code a solution for Vero's problem.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">The solution to this is to count the lines of code that are between the label and the goto statement, having in consideration that the goto will always <em>return</em> to an existent label, the label will consist on a single string formed by letters from the 'a' to the 'z' and from the 'A' to the 'Z', all labels will have the format <em><span style="text-decoration: underline;">&lt;label&gt;:</span></em> as the goto will always contains the format <em><span style="text-decoration: underline;">goto &lt;label&gt;;</span></em>, however, remember that before the labels and the gotos you can have an important amount of spaces that will count as an indentation of a code.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Note: An uppercase letter label is distinct from a lowercase letter label, by example: 'abc' is not equal to 'ABC'</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>INPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">The first line of input will contain an integer T denoting the T test cases, then, T cases will follow. Each of the following line will contain an integer N, then, N lines will follow, each of the next N lines will contain a string S.</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>OUTPUT:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">Output the string ��Scenario #i: �� where i is the test case you are analyzing followed by the sum of the number of lines between the label and the goto.</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<p style="margin-bottom: 0in;">SAMPLE DATA:</p>
<p style="margin-bottom: 0in;">&nbsp;</p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><strong>INPUT</strong></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><strong>OUTPUT</strong></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p>3</p>
<p>6</p>
<p>A:</p>
<p>&nbsp; &nbsp; &nbsp; SPACES will InDeNt the CoDe</p>
<p>&nbsp; &nbsp; &nbsp; No TaBs ArE iN the &gt;&gt; test &lt;&lt; data</p>
<p>goto A;</p>
<p>B:</p>
<p>goto B;</p>
<p>7</p>
<p>B:</p>
<p>A:</p>
<p>cin &gt;&gt; n;</p>
<p>&nbsp; &nbsp; if(n&lt;0) then</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;goto A;</p>
<p>&nbsp; &nbsp; else</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;goto B;</p>
<p><span style="white-space: pre-wrap;">7</span></p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;A:</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;TumbaBicho:</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;printf("goto TumbaBicho");</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp;printf("goto TumbaBicho");</p>
<p>&nbsp; &nbsp; &nbsp;goto TumbaBicho;</p>
<p>AA:</p>
<p>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;goto A;</p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p>Scenario #1: 2</p>
<p>Scenario #2: 7</p>
<p>Scenario #3: 7</p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><strong>CONSTRAINTS:</strong></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">1&lt;=N&lt;=10000</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">1&lt;= Length of string &lt;= 1000</p>