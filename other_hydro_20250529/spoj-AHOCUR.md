<p><span style="font-family: sans-serif; font-size: 13px; line-height: 19px;">The&nbsp;</span><strong>Aho�CCorasick string matching algorithm</strong><span style="font-family: sans-serif; font-size: 13px; line-height: 19px;">&nbsp;is a&nbsp;</span><a style="text-decoration: none; color: #0b0080; background-image: none; font-family: sans-serif; font-size: 13px; line-height: 19px;" title="String searching algorithm" href="http://en.wikipedia.org/wiki/String_searching_algorithm">string searching algorithm</a><span style="font-family: sans-serif; font-size: 13px; line-height: 19px;">&nbsp;invented by&nbsp;</span><a style="text-decoration: none; color: #0b0080; background-image: none; font-family: sans-serif; font-size: 13px; line-height: 19px;" title="Alfred V. Aho" href="http://en.wikipedia.org/wiki/Alfred_V._Aho">Alfred V. Aho</a><span style="font-family: sans-serif; font-size: 13px; line-height: 19px;">&nbsp;and&nbsp;</span><a style="text-decoration: none; color: #0b0080; background-image: none; font-family: sans-serif; font-size: 13px; line-height: 19px;" title="Margaret J. Corasick" href="http://en.wikipedia.org/wiki/Margaret_J._Corasick">Margaret J. Corasick</a><span style="font-family: sans-serif; font-size: 13px; line-height: 19px;">. It is a kind of dictionary-matching algorithm that locates elements of a finite set of strings (the "dictionary") within an input text. It matches all patterns simultaneously. &nbsp;</span></p>
<p>The Algorithm described above, requires an input file generator. The generator generates a text of length&nbsp;<em>L</em>, by choosing&nbsp;<em>L</em>&nbsp;characters randomly. Probability of choosing each character is given as priori, and independent of choosing others. &nbsp;Now, given a set of patterns, calculate the probability of a valid program generating ��no��.</p>
<h3>Input</h3>
<p>First line contains an integer&nbsp;<em>T</em>, the number of test cases. Each case starts with an integer&nbsp;<em>K</em>, the number of pattern strings. Next&nbsp;<em>K</em>&nbsp;lines each contain a pattern string, followed by an integer&nbsp;<em>N</em>, number of valid characters.&nbsp;&nbsp;Next&nbsp;<em>N</em>&nbsp;lines each contain a character and the probability of selecting that character,&nbsp;<em>p<sub>i</sub></em>. Next an integer&nbsp;<em>L</em>, the length of the string generated. The generated text can consist of only the valid characters, given above. &nbsp;There will be a blank line after each test case.</p>
<h3>Output</h3>
<p>For each test case, output the number of test case, and the probability of getting a ��no��.</p>
<p><strong>Constraints</strong></p>
<ul>
<li>T&nbsp;&nbsp;�� 100</li>
<li>K �� 40</li>
<li>Length of each pattern string is between 1 and 20</li>
<li>Each pattern string consists of only alphanumeric characters (��a�� to ��z��, ��A�� to ��Z��,��0�� to ��9��)</li>
<li>Valid characters are all alphanumeric characters</li>
<li>��p<sub>i&nbsp;</sub>= 1</li>
<li>L �� 100</li>
</ul>
<h3>Example</h3>
<pre><strong>Input</strong><span style="white-space: normal;">&nbsp;</span></pre>
<pre>2
1
a
2
a 0.5
b 0.5
2
 
2
ab
ab
2
a 0.2
b 0.8
2<strong>

</strong></pre>
<pre><strong>Output:</strong></pre>
<pre>Case #1: 0.250000
Case #2: 0.840000</pre>
<pre><strong><div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">1</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">a 0.5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">b 0.5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">ab</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">ab</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">a 0.2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">b 0.8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 380px; width: 1px; height: 1px; overflow: hidden;">2</div>
<br></strong></pre>