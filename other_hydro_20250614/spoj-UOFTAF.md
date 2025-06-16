<p>
<script type="text/x-mathjax-config">// <![CDATA[
MathJax.Hub.Config({tex2jax: {inlineMath: [['$','$'], ['\\(','\\)']]}});
// ]]></script>
<script src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
</p>
<p>Let's talk about some definitions, shall we?</p>
<p>An uppercase letter is a character between "A'' and "Z'', inclusive. You knew that.</p>
<p>A string is a sequence of characters. You probably knew that.</p>
<p>A Foxic letter is a superior uppercase letter - namely, one of "F", "O", or "X". You probably didn't know that.</p>
<p>A Foxic string is a superior string, consisting only of Foxic letters. You didn't know that.</p>
<p>Finally, a Foxic expression is a special string, with each of its characters being either a Foxic letter, or an "n" immediately following a Foxic letter. A Foxic expression can be translated into a Foxic string by a three-step process. First, up to one character can be added, removed, or modified, provided that the resulting string is still a valid Foxic expression. Next, every Foxic letter immediately preceding an "n" is replaced by zero or more occurrences of that same letter. Finally, each "n" is removed. You most certainly did not know that.</p>
<p>There are $T$ ($1 \leq T \leq 100$) scenarios to consider, as described above. In each scenario, given a Foxic string $S$ of length $N$ ($1 \leq N \leq 100$) and a Foxic expression $E$ of length $M$ ($1 \leq M \leq 100$), you'd like to determine whether or not $E$ can be translated into $S$.</p>
<h3>Input</h3>
<p>Line 1: 1 integer, $T$</p>
<p>For each scenario:</p>
<p>Line 1: 1 integer, $N$</p>
<p>Line 2: 1 string, $S$</p>
<p>Line 3: 1 integer, $M$</p>
<p>Line 4: 1 string, $E$</p>
<h3>Output</h3>
<p>For each scenario:</p>
<p>The string "Yes" (without quotes) if $E$ can be translated into $S$, or "No" otherwise.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">2<br>5<br>OOOFO<br>7<br>OXnFOXn<br>3<br>FOX<br>7<br>OFnOXnO</span>

<strong>Output:</strong></pre>
<pre><span style="font-family: 'courier new', courier;">Yes<br>No</span></pre>
<pre><strong>Explanation of Sample:</strong></pre>
<p>In the first scenario, one possible course of action is to erase the second character of $E$, leaving the Foxic expression "OnFOXn". Next, we may choose to replace the first "O" with three copies of "O", and the remaining "X" with zero occurrences of "X", since each of these precedes an "n" - this yields the string "OOOnFOn". Finally, after removing each "n", we are left with "OOOFO", which matches $S$. Replacing the second character with an "O" would have also been possible.</p>
<p>In the second scenario, it is impossible to translate $E$ into $S$ through any valid steps.</p>