<p>ACM ICPC World Finals 2009, sponsored by IBM and hosted by KTH, Royal Institute of Technology will be held in Stockholm, Sweden. This contest will last for <em>N</em>(1&lt;= <em>N</em> &lt;= 1000) days. We need at least <em>A<sub>i</sub></em> volunteers in the <em>i</em>-th day. Now there are <em>M</em>(1&lt;= <em>M</em> &lt;=10000) kind of volunteers. The <em>i</em>-th type of volunteers will work from <em>S<sub>i</sub></em>-th day to <em>T<sub>i</sub></em>-th day, we will pay them $<em>C<sub>i</sub></em>. Now your task is to minimize the money KTH pay for all the volunteers.</p>
<h3>Input</h3>
<p>Ten test cases(given one after another, you have to process all!). For each test case:</p>
<p>The first line contains two space-seperated integers <em>N</em> and <em>M</em>. The second line contains N nonnegative integers <em>A<sub>i</sub></em>. <em>M</em> lines follow, each contains three integers <em>S<sub>i</sub></em>, <em>T<sub>i</sub></em> and <em>C<sub>i</sub></em>. You may assume you can hire almost unlimited number of every type of volunteers.</p>
<p><em>Tip</em>: During your calculation, <strong>int</strong> in C/C++/Java or <strong>longint</strong> in Pascal is enough.</p>
<h3>Output</h3>
<p>For each test case:</p>
<p>Output one line with an integer - the minimum cost.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 3
2 3 4
1 2 2
2 3 5
3 3 2
[and 9 test cases more]

<strong>Output:</strong>
14
[and 9 test cases more]
</pre>