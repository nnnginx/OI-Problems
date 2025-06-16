<p>Let A = a<sub>1</sub>a<sub>2</sub>...a<sub>k</sub> and B = b<sub>1</sub>b<sub>2</sub>...b<sub>l</sub> be strings of lengths
k and l,
respectively. The string distance between A and B is defined in the
following
way (d[i,j] is the distance of substrings a<sub>1</sub>...a<sub>i</sub> and b<sub>1</sub>...b<sub>j</sub>, where 0 ¡Ü i ¡Ü k and 0 ¡Ü j ¡Ü l -- i or j being 0
represents the empty substring). The definition for d[i, j] is d[0, 0] = 0 and for (i, j) ¡Ù (0, 0) d[i, j] is the minimum of all that apply:
</p><ul>
<li>d[i, j - 1] + 1, if j &gt; 0</li>
<li>d[i - 1, j] + 1, if i &gt; 0</li>
<li>d[i - 1, j - 1], if i &gt; 0, j &gt; 0, and a<sub>i</sub> = b<sub>j</sub></li>
<li>d[i - 1, j - 1] + 1, if i &gt; 0, j &gt; 0, and a<sub>i</sub> ¡Ù b<sub>j</sub></li>
<li>d[i - 2, j - 2] + 1, if i ¡Ý 2, j ¡Ý 2, a<sub>i</sub> = b<sub>j-1</sub>, and a<sub>i-1</sub> = b<sub>j</sub></li>
</ul>

<p>The distance between A and B is equal to d[k,l].

</p><p>For two given strings A and B, compute their distance knowing that it is not higher than 100.

</p><h3>Input</h3>
<p>In the first line, k and l are given, giving the lengths of the strings
A and
B (1 ¡Ü k, l ¡Ü 10<sup>5</sup>). In the second and third lines strings A and
B, respectively, are given.  A and B contain only lowercase
letters of the English alphabet.

</p><h3>Output</h3>
<p>In the first line, write one number, the distance between A and B,
followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
8 8
computer
kmpjutre

<b>Output:</b>
4
</pre>