<p>Ada the Ladybug is helping her friend who is biologist. He examines DNA. Actually he has a long DNA of one bug, consisting of adenine, cytosine, guanine and thymine and he wants to know whether another bug might be relative to first bug. A bug is relative to another bug if his his DNA has very low Hamming Distance with some substring of the first bug.</p>
<p>Your job is to find the lowest hamming distance between second DNA and any substring of first DNA.</p>
<h3>Input</h3>
<p>Input contains only two lines: first DNA (<strong>s</strong>) and second DNA (<strong>r</strong>).</p>
<p>It is true that <strong>0 &lt; |r| ¡Ü |s| ¡Ü 5*10<sup>5</sup></strong></p>
<p><strong>|s|</strong> means leangth of string <strong>s</strong>.</p>
<p>All strings contains only <strong>A, C, T, and G</strong> .</p>
<h3>Output</h3>
<p>Print minimal <a href="https://en.wikipedia.org/wiki/Hamming_distance">Hamming     Distance</a> (the number of mismatched nucleobases) of any substring of <strong>s</strong> and <strong>r</strong> (the substring MUST have length <strong>|r|</strong>)</p>
<h3>Example Inputs</h3>
<pre>ACTGACTGACTG
ACCG
</pre>
<pre>AAAAAACCA
AAACA
</pre>
<pre>ACGC
GGG
</pre>
<pre>ACTTTG
TTTGA
</pre>
<pre>ACTGACTGACTG
ACTG
</pre>
<h3>Example Output</h3>
<pre>1
</pre>
<pre>1
</pre>
<pre>2
</pre>
<pre>3
</pre>
<pre>0
</pre>
<h3>Inputs explanation</h3>
<pre><span style="color: red;"><strong>ACTG</strong></span>ACTGACTG
AAAA<span style="color: red;"><strong>AACCA</strong></span>
A<span style="color: red;"><strong>CGC</strong></span>
A<span style="color: red;"><strong>CTTTG</strong></span>
ACTG<span style="color: red;"><strong>ACTG</strong></span>ACTG 

</pre>