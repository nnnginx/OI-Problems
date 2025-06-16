<p>Blue Mary, the queen of Protoss, is planning a war against Zerg. Before the war she plans to make her base as safe as possible. Now there are <em>N</em> (1&lt;= <em>N</em> &lt;= 60) nexuses available in the region controlled by Protoss, numbered 1, 2, ..., <em>N</em>. (Those who don't know what nexus is, please visit <a href="http://www.blizzard.com">Blizzard Entertainment</a>.) All the mineral and vespene gas stored in nexus <em>i</em> can be transported directly to nexus <em>S<sub>i</sub></em>.(<em>i</em> and <em>S<sub>i</sub></em> won't be the same.) Blue Mary's base is nexus 1, So all the mineral and vespene gas can be transported to base 1 directly or indirectly.</p>
<p>Blue Mary defines the safety of nexus <em>i</em>, <strong>R(i)</strong>, as the following:</p>
<p><img src="./24724/file/im9jadYK.png" alt=""></p>
<p><em>C<sub>i</sub></em> and <em>k</em> are numeral constants which will be given in the input file.</p>
<p>Suppose for a fixed <em>i</em>, set T={P<sub>1</sub>, P<sub>2</sub>, P<sub>3</sub>, ..., P<sub>w</sub>}, then <strong>x</strong> is a member of T if and only if S<sub><strong>x</strong></sub> is <em>i</em>. Any two P<sub>j</sub>s must be different.</p>
<p>Now Blue Mary wants to modify at most <em>M</em> (0&lt;= <em>M</em> &lt;= <em>N</em>) <em>S<sub>i</sub></em> s, so that the safety of her base <strong>R(1)</strong> is maximized. To be a terran captive, also a great programmer, you must help her to solve this problem. Price is your life. Be careful! Blue Mary tells you that <em>S<sub>1</sub></em> can't be modified. Don't ask your queen about the reason please.</p>
<h3>Input</h3>
<p>Ten test cases(given one after another, you have to process all!). For each test case:</p>
<p>The first line contains <em>N</em>, <em>M</em> and a real number <em>k</em> (0.3&lt;= <em>k</em> &lt;1). The second line contains <em>N</em> space seperated integers <em>S<sub>i</sub></em>. The third line contains <em>N</em> positive real numbers <em>C<sub>i</sub></em>.</p>
<p>There is a single blank line between consecutive test cases.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>A single line - the maximized safety of nexus 1, rounded to two decimal places.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 1 0.5
2 3 1 3
10.0 10.0 10.0 10.0</pre>
<pre>[and 9 test cases more]

<strong>Output:</strong>
30.00
[and 9 test cases more]
</pre>
<h3>Hint</h3>
<p>Before modifying, the safety of the 4 bases are 22.8571, 21.4286,25.7143,10, respectively.</p>
<p>After modifying <em>S<sub>2</sub></em> to 1, the safety of the 4 bases are 30, 25, 15, 10, respectively.</p>