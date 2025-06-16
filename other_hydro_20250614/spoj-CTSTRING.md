<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A regular expression is used to describe a set of strings. For this problem the alphabet is limited to 'a' and 'b'. R is a regular expression if:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1) R is "a" or "b"</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2) R is of the form "(R1R2)" where R1 and R2 are regular expressions</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3) R is of the form "(R1|R2)" where R1 and R2 are regular expressions</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4) R is of the form "(R1*)" where R1 is a regular expression.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The set of strings recognised by R are as follows:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1) If R is "a", then the set of strings recognised = {a}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2) If R is "b", then the set of strings recognised = {b}</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3) if R is of the form "(R1R2)" then the set of strings recognised = all strings which can be obtained by a concatenation of strings s1 and s2 where s1 is recognised by R1 and s2 by R2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4) if R is of the form "(R1|R2)" then the set of strings recognised = union of the set of strings recognised by R1 and R2.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5) If R is of the form "(R1*)" then the the strings recognised are the empty string and the concatenation of an arbitrary number of copies of any string recognised by R1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given a regular expression and an integer L, you need to count how many strings of length L are recognized by it.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T test cases follow.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each test case contains a regular expression R and an integer L.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines one corresponding to each test case containing the required answer for the corresponding test case. As the answers can be very big, output them modulo 1000000007.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= length(R) &lt;= 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= L &lt;= 10^9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are guaranteed that R will conform to the definition provided above.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">((ab)|(ba)) 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">((a|b)*) 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">((a*)(b(a*))) 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">32</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Explanation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the first case, the only strings recognized are "ab" and "ba".</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the second case, the regex recognizes any string containing only a's and b's. So the number of strings of length 5 recognized by it is 2^5 = 32.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the third case, the regex recognizes any string having one b, preceeded and followed by any number of a's. Clearly, there are 100 strings of length 100 which have a single b in them.</div>
<p>&nbsp;</p>
<p>A regular expression is used to describe a set of strings. For this problem the alphabet is limited to 'a' and 'b'. R is a regular expression if:</p>
<p>1) R is "a" or "b"</p>
<p>2) R is of the form "(R1R2)" where R1 and R2 are regular expressions</p>
<p>3) R is of the form "(R1|R2)" where R1 and R2 are regular expressions</p>
<p>4) R is of the form "(R1*)" where R1 is a regular expression.</p>
<p>&nbsp;</p>
<p>The set of strings recognised by R are as follows:</p>
<p>1) If R is "a", then the set of strings recognised = {a}</p>
<p>2) If R is "b", then the set of strings recognised = {b}</p>
<p>3) if R is of the form "(R1R2)" then the set of strings recognised = all strings which can be obtained by a concatenation of strings s1 and s2 where s1 is recognised by R1 and s2 by R2.</p>
<p>4) if R is of the form "(R1|R2)" then the set of strings recognised = union of the set of strings recognised by R1 and R2.</p>
<p>5) If R is of the form "(R1*)" then the the strings recognised are the empty string and the concatenation of an arbitrary number of copies of any string recognised by R1.</p>
<p>&nbsp;</p>
<p>Given a regular expression and an integer L, you need to count how many strings of length L are recognized by it.</p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>The first line contains the number of test cases T. T test cases follow.&nbsp;</p>
<p>Each test case contains a regular expression R and an integer L.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>Output T lines one corresponding to each test case containing the required answer for the corresponding test case. As the answers can be very big, output them modulo 1000000007.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 50</p>
<p>1 &lt;= length(R) &lt;= 100</p>
<p>1 &lt;= L &lt;= 10^9</p>
<p>You are guaranteed that R will conform to the definition provided above.</p>
<p>All inputs will be randomly generated.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>3</p>
<p>((ab)|(ba)) 2</p>
<p>((a|b)*) 5</p>
<p>((a*)(b(a*))) 100</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2</p>
<p>32</p>
<p>100</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p>For the first case, the only strings recognized are "ab" and "ba".</p>
<p>For the second case, the regex recognizes any string containing only a's and b's. So the number of strings of length 5 recognized by it is 2^5 = 32.</p>
<p>For the third case, the regex recognizes any string having one b, preceeded and followed by any number of a's. Clearly, there are 100 strings of length 100 which have a single b in them.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>