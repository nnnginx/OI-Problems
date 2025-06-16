<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A regular expression is a string which contains some normal characters and some meta characters.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The meta characters include,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">. means any character</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">[c1 − c2]means any character between c1 and c2 (c1 and c2 are two characters)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">[ ˆ c1 − c2] means any character not between c1 and c2 (c1 and c2 are two characters)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;"> means the character before it can occur any times</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">+ means the character before it can occur any times but at least one times</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">\ means any character follow should be treated as normal character</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are to write a program to find the leftmost substring of a given string, so that the substring</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">can match a given regular expression. If there are many substrings of the given string can match</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">the regular expression, and the left positions of these substrings are same, we prefer the longest</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">one.</div>
<p>&nbsp;</p>
<div style="text-align: justify; ">A regular expression is a string which contains some normal characters and some meta characters.</div>
<div style="text-align: justify; ">The meta characters include,</div>
<div style="text-align: justify; ">. means any character</div>
<div style="text-align: justify; ">[c1 − c2]means any character between c1 and c2 (c1 and c2 are two characters)</div>
<div style="text-align: justify; ">[ ˆ c1 − c2] means any character not between c1 and c2 (c1 and c2 are two characters)</div>
<div style="text-align: justify; "> means the character before it can occur any times</div>
<div style="text-align: justify; ">+ means the character before it can occur any times but at least one times</div>
<div style="text-align: justify; ">\ means any character follow should be treated as normal character</div>
<div style="text-align: justify; ">You are to write a program to find the leftmost substring of a given string, so that the substring&nbsp;can match a given regular expression. If there are many substrings of the given string can match&nbsp;the regular expression, and the left positions of these substrings are same, we prefer the longest&nbsp;one.</div>
<div style="text-align: justify; "></div>
<h3>Input</h3>
<div style="text-align: justify;">Every two lines of the input is a pattern-matching problem. The first line is a regular expression,&nbsp;and the second line is the string to be matched. Any line will be no more than 80 character. A line&nbsp;with only an eEvery two lines of the input is a pattern-matching problem. The first line is a regular expression,&nbsp;and the second line is the string to be matched. Any line will be no more than 80 character. A line&nbsp;with only an end will terminate the input.nd will terminate the input.</div>
<h3>Output</h3>
<p>&nbsp;</p>
<div style="text-align: justify;">For each matching problem, you should give an answer in one line. This line contains the string to&nbsp;be matched, but the leftmost substring that can match the regular expression should be bracketed.&nbsp;If no substring matches the regular expression, print the input string.</div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre style="text-align: justify;"><strong>Input:</strong>

.*
asdf
f.*d.
sefdfsde
[0-9]+
asd345dsf
[^\*-\*]
**asdf**fasd
b[a-z]*r[s-u]*
abcdefghijklmnopqrstuvwxyz
[T-F]
dfkgjf
end</pre>
<pre style="text-align: justify;"><strong>Output:</strong></pre>
<pre style="text-align: justify;">(asdf)
se(fdfsde)
asd(345)dsf
**(a)sdf**fasd
a(bcdefghijklmnopqrstu)vwxyz
dfkgjf</pre>
<pre style="text-align: justify;"></pre>