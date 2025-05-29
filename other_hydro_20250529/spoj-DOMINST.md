<p><span style="font-size: medium;"><strong>Dominant Strings</strong></span></p>
<p style="margin-right: 0in; margin-left: 0in; font-size: medium; font-family: 'Arial Unicode MS'; text-align: justify;"><span style="font-family: 'Times New Roman';">Given two strings&nbsp;<em>s<sub>1</sub></em>&nbsp;and&nbsp;<em>s<sub>2</sub></em>, we say that&nbsp;<em>s<sub>1</sub></em>&nbsp;<em>dominates</em>&nbsp;<em>s<sub>2</sub></em>&nbsp;if the (multi)set of characters in&nbsp;<em>s<sub>1</sub></em>&nbsp;is a proper superset of the (multi)set of characters in&nbsp;<em>s<sub>2</sub></em>. For instance, "acmicpc" dominates "camp", but it does not dominate "chimp" or "macpac". For a set&nbsp;<em>S</em>&nbsp;of strings, we call the strings in&nbsp;<em>S</em>&nbsp;which are not dominated by any string in&nbsp;<em>S</em>&nbsp;the<em>dominant strings</em>&nbsp;of&nbsp;<em>S</em>&nbsp;(even if they do not dominate any strings in&nbsp;<em>S</em>).</span></p>
<p style="margin-right: 0in; margin-left: 0in; font-size: medium; font-family: 'Arial Unicode MS'; text-align: justify;"><span style="font-family: 'Times New Roman';">Now, your task is simply to find all the dominant strings of a set of strings.</span></p>
<h3>Input</h3>
<p><span style="font-family: 'Times New Roman'; font-size: 16px; text-align: justify;">The input contains a single set of strings, with one string per line. Each string consists of at least one and at most ten lower-case alphabetic characters. There will be at most 15000 strings, and no two strings will be identical. Input is terminated by end-of-file.</span></p>
<p style="margin-right: 0in; margin-left: 0in; font-size: medium; font-family: 'Arial Unicode MS'; text-align: justify;"><strong>Output</strong></p>
<p><span style="font-family: 'Times New Roman'; font-size: 16px; text-align: justify;">Output consists of all dominant strings in the input set, in alphabetical order, one word per line.</span></p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<p>acmicpc<br>cccp<br>macpac<br>chimp<br>camp</p>
<p><span style="font-weight: bold; ">Output:</span></p>
<p>acmicpc<br>chimp<br>macpac</p>
<p>&nbsp;</p>