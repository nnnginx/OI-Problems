<p>You are given a string T which consists of 40000 lowercase latin letters at most. You are also given some integers A, B and Q. You have to answer Q queries. For i-th query you are given a string S<sub><span style="font-size: xx-small;">i</span></sub> and you need to output how many times S<sub>i</sub> appears in T. Immediately after answering the current query you need to add ((A*ans+B) modulo 26+1)-th lowercase symbol of the English alphabet to the end of T where ans is the answer to this query.</p>
<h3>Input</h3>
<p>The first line of input contains a string T. The next line consists of three integers Q (1&lt;=Q&lt;=40000), A (0&lt;=A&lt;=27) and B (0&lt;=B&lt;=26). The following Q lines contain Q query strings, S<sub>i-2</sub> on i-th line. Input will not exceed 600 kb.</p>
<h3>Output</h3>
<p>Output Q lines. Output the answer to the i-th query on the i-th line output.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>aaaaa<br>2 0 0<br>a<br>aa<br><br><strong>Output:</strong><br>5<br>5<br></pre>