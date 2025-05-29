<p>In the year 29XX, the government of a small country somewhere on the earth introduced a law restricting first names of the people only to traditional names in their culture, in order to preserve their cultural uniqueness.  The linguists of the country specifies a set of rules once every year, and only names conforming to the rules are allowed in that year.  In addition, the law also requires each person to use a name of a specific length calculated from one's birth date because otherwise too many people would use the same very popular names.  Since the legislation of that law, the common task of the parents of new babies is to find the name that comes first in the alphabetical order among the legitimate names of the given length because names earlier in the alphabetical order have various benefits in their culture.</p>
<p>Legitimate names are the strings consisting of only lowercase letters that can be obtained by repeatedly applying the rule set to the initial string ``S'', a string consisting only of a single uppercase S.</p>
<p>Applying the rule set to a string is to choose one of the rules and apply it to the string.  Each of the rules has the form  <span><em>A</em> <img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"> <img src="/content/zukow:BABY_alpha.png" border="0" alt="$ \alpha$" width="16" height="15" align="BOTTOM"></span>, where <span><em>A</em></span> is an uppercase letter and <span><img src="/content/zukow:BABY_alpha.png" border="0" alt="$ \alpha$" width="16" height="15" align="BOTTOM"></span> is a string of lowercase and/or uppercase letters.  Applying such a rule to a string is to replace an occurrence of the letter <span><em>A</em></span> in the string to the string <span><img src="/content/zukow:BABY_alpha.png" border="0" alt="$ \alpha$" width="16" height="15" align="BOTTOM"></span>.  That is, when the string has the form `` <span><img src="/content/zukow:BABY_beta.png" border="0" alt="$ \beta$" width="15" height="33" align="MIDDLE"><em>A</em><img src="/content/zukow:BABY_gamma.png" border="0" alt="$ \gamma$" width="14" height="31" align="MIDDLE"></span>'', where <span><img src="/content/zukow:BABY_beta.png" border="0" alt="$ \beta$" width="15" height="33" align="MIDDLE"></span> and <span><img src="/content/zukow:BABY_gamma.png" border="0" alt="$ \gamma$" width="14" height="31" align="MIDDLE"></span> are arbitrary (possibly empty) strings of letters, applying the rule rewrites it into the string `` <span><img src="/content/zukow:BABY_beta.png" border="0" alt="$ \beta$" width="15" height="33" align="MIDDLE"><img src="/content/zukow:BABY_alpha.png" border="0" alt="$ \alpha$" width="16" height="15" align="BOTTOM"><img src="/content/zukow:BABY_gamma.png" border="0" alt="$ \gamma$" width="14" height="31" align="MIDDLE"></span>''.  If there are two or more occurrences of <span><em>A</em></span> in the original string, an arbitrary one of them can be chosen for the replacement.</p>
<p>Below is an example set of rules.</p>
<blockquote>
<table border="0">
<colgroup><col align="CENTER"><col align="CENTER"><col align="LEFT"><col align="CENTER"><col align="LEFT"> 
</colgroup><tbody>
<tr>
<td align="CENTER" valign="BASELINE">S</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">aAB</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(1)</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">A</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td><br></td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(2)</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">A</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">Aa</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(3)</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">B</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">AbbA</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(4)</td>
</tr>
</tbody>
</table>
</blockquote>
<p>Applying the rule (1) to ``S'', ``aAB'' is obtained.  Applying (2) to it results in ``aB'', as A is replaced by an empty string.  Then, the rule (4) can be used to make it ``aAbbA''.  Applying (3) to the first occurrence of A makes it ``aAabbA''.  Applying the rule (2) to the A at the end results in ``aAabb''.  Finally, applying the rule (2) again to the remaining A results in ``aabb''.  As no uppercase letter remains in this string, ``aabb'' is a legitimate name.</p>
<p>We denote such a rewriting process as follows.</p>
<blockquote>S <span>&nbsp;<img src="/content/zukow:BABY_arrow1.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (1)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aAB <span>&nbsp;<img src="/content/zukow:BABY_arrow2.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (2)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aB <span>&nbsp;<img src="/content/zukow:BABY_arrow4.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (4)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aAbbA <span>&nbsp;<img src="/content/zukow:BABY_arrow3.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (3)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aAabbA  <span>&nbsp;<img src="/content/zukow:BABY_arrow2.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (2)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aAabb <span>&nbsp;<img src="/content/zukow:BABY_arrow2.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (2)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>aabb</blockquote>
<p>Linguists of the country may sometimes define a ridiculous rule set such as follows.</p>
<blockquote>
<table border="0">
<colgroup><col align="CENTER"><col align="CENTER"><col align="LEFT"><col align="CENTER"><col align="LEFT"> 
</colgroup><tbody>
<tr>
<td align="CENTER" valign="BASELINE">S</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">sA</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(1)</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">A</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">aS</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(2)</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">B</td>
<td align="CENTER" valign="BASELINE"><span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span></td>
<td align="LEFT" valign="BASELINE">b</td>
<td><br></td>
<td align="LEFT" valign="BASELINE">(3)</td>
</tr>
</tbody>
</table>
</blockquote>
<p>The only possible rewriting sequence with this rule set is:</p>
<blockquote>S <span>&nbsp;<img src="/content/zukow:BABY_arrow1.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (1)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>sA <span>&nbsp;<img src="/content/zukow:BABY_arrow1.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (2)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>saS <span>&nbsp;<img src="/content/zukow:BABY_arrow1.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (1)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span>sasA <span>&nbsp;<img src="/content/zukow:BABY_arrow1.png" border="0" alt="$ \;\stackrel{{\mbox{\tiny (2)}}}{{\longrightarrow}}\;$" width="42" height="25" align="BOTTOM"> &nbsp;</span><span><sup> ... </sup></span></blockquote>
<p>which will never terminate.  No legitimate names exist in this case. Also, the rule (3) can never be used, as its left hand side, B, does not appear anywhere else.</p>
<p>It may happen that no rules are supplied for some uppercase letters appearing in the rewriting steps.  In its extreme case, even S might have no rules for it in the set, in which case there are no legitimate names, of course.  Poor nameless babies, sigh!</p>
<p>Now your job is to write a program that finds the name earliest in the alphabetical order among the legitimate names of the given length conforming to the given set of rules.</p>
<h3>Input</h3>
<p>The input is a sequence of datasets, followed by a line containing two zeros separated by a space representing the end of the input.  Each dataset starts with a line including two integers <span><em>n</em></span> and <span><em>l</em></span> separated by a space, where <span><em>n</em></span> (0 &lt;= <span><em>n</em></span> &lt;= 50) is the number of rules and <span><em>l</em></span> (0 &lt;= <span><em>l</em></span> &lt;= 20) is the required length of the name. After that line, <span><em>n</em></span> lines each representing a rule follow.  Each of these lines starts with one of uppercase letters, A to Z, followed by the character ``='' (instead of `` <span><img src="/content/zukow:BABY_arrow.png" border="0" alt="$ \rightarrow$" width="22" height="17" align="BOTTOM"></span>'') and then followed by the right hand side of the rule which is a string of letters A to Z and a to z.  The length of the string does not exceed 10 and may be zero.  There appears no space in the lines representing the rules.</p>
<h3>Output</h3>
<p>The output consists of the lines showing the answer to each dataset in the same order as the input.  Each line is a string of lowercase letters, a to z, which is the first legitimate name conforming to the rules and the length given in the corresponding input dataset.  When the given set of rules has no conforming string of the given length, the corresponding line in the output should show a single hyphen, ``<tt>-</tt>''.  No other characters should be included in the output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>&nbsp;<pre>4 3
A=a
A=
S=ASb
S=Ab
2 5
S=aSb
S=
1 5
S=S
1 0
S=S
1 0
A=
2 0
A=
S=AA
4 5
A=aB
A=b
B=SA
S=A
4 20
S=AAAAAAAAAA
A=aA
A=bA
A=
0 0
</pre>
<strong>Output:</strong>&nbsp;
<pre>abb
-
-
-
-

aabbb
aaaaaaaaaaaaaaaaaaaa
</pre>
</pre>