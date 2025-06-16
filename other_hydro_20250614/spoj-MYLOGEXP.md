<p>Cho decided that it is time to find the love of his life. After conducting intensive online research, he found out that to stand a chance, he has to be intelligent, handsome, kind, charismatic, confident, funny, responsible, reliable, straightforward, mysterious, a gentleman.....</p>
<p>Cho was puzzled. He thought he already had all of these characteristics. After taking a definitely legitimate online personality test, he realized he lacked just one of them - he was not mysterious enough.</p>
<p>He decided he will only say statements with as many interpretations as possible; that way it will always be unclear what he actually means, and that should grant him an aura of unpredictability and mysteriousness.&nbsp;</p>
<p>Cho prepared some pickup lines, and now he wants to know how mysterious they sound - that is, how many ways they can be interpreted to still make sense.</p>
<h3>Input</h3>
<p>Each pickup line can be represented by a logical expression. A valid logical expression <strong>exp</strong> can be</p>
<ul>
<li><strong>exp = X</strong></li>
<li><strong>exp = OR(exp,exp)</strong></li>
<li><strong>exp = AND(exp,exp)</strong></li>
<li><strong>exp = NOT(exp)</strong></li>
</ul>
<p>where&nbsp;<strong>X&nbsp;</strong>is a boolean variable, and&nbsp;<strong>OR</strong>, <strong>AND</strong>, <strong>NOT</strong>&nbsp;are <a href="https://en.wikipedia.org/wiki/Boolean_algebra#Basic_operations">basic boolean operations</a>.</p>
<p>&nbsp;</p>
<p>The first line contains an integer <strong>1 ¡Ü T </strong><strong>¡Ü 6</strong>, the number of expressions.</p>
<p>Each of the <strong>T&nbsp;</strong>subsequent lines contains one valid expression as described above (i.e. it is correctly parenthesized, with no additional spaces).</p>
<p><strong>|exp|</strong>&nbsp;<strong>¡Ü 700,000</strong>&nbsp;and the sum of <strong>|exp| </strong>in an input file <strong>¡Ü 1,850,000</strong></p>
<h3>Output</h3>
<p>For each expression, find the number of ways that True/False values can be (independently) assigned to the variables <strong>X</strong>&nbsp;in the expression so that the whole expression evaluates to True.</p>
<p>Since this value could be huge, output it modulo <strong>10<sup>9</sup>+7</strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
AND(X,OR(X,X))
NOT(OR(X,X))

<strong>Output:</strong>
3
1
</pre>