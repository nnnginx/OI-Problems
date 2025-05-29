<p><span style="font-size: small;">A far away galaxy, H10 has newly been discovered and incorporated into the Commonwealth which participates in the Galactic Wars. The other galaxies have always bullied it by winning the Galactic Wars every year. Frustrated, H10 has come up with a novel strategy to distract the other galaxies. They are planning to send beautiful nymphs into the lands of the other galaxies.</span></p>
<p><span style="font-size: small;">The cosmos is arranged so that there is a unique&nbsp;path between any two galaxies (possibly going through other galaxies). The leaders in H10 will select two different galaxies A and B, and send K nymphs to each of the galaxies that is on the unique path from A to B. Initially there are no nymphos on any galaxy.</span></p>
<p><span style="font-size: small;">You are the Chief Executive Officer of this project. The leaders will ask you to send these groups of nymphs by giving various instructions of the form (A,B,K). In the process, they may also ask you how many nymphs are currently there in particular galaxies, so that they are able to take smart decisions in the future. Implement this. (See exact format in Input/Output Specifications)</span></p>
<h3><span style="font-size: small;">Input</span></h3>
<p><span style="font-size: small;">The first line contains t, the number of test cases.</span></p>
<p><span style="font-size: small;">T test cases follow. Each contains :</span></p>
<p><span style="font-size: small;">A line containing n, the number of galaxies (numbered from 0 to n-1).&nbsp;</span></p>
<p><span style="font-size: small;">n-1 lines describing the connections between 2 galaxies as 2 space separated integers a, b (both from 0 to n-1), denoting a direct connection between galaxy a, and galaxy b.</span></p>
<p><span style="font-size: small;">The next line contains a single integer Q denoting the number of queries.</span></p>
<p><span style="font-size: small;">Next Q lines contain queries in the form of 3 space separated integers a, b and k.</span></p>
<h3><span style="font-size: small;">Output</span></h3>
<p><span style="font-size: small;">For each query if k&gt;=0, don't output anything, just send the nymphos to every galaxy on the way.</span></p>
<p><span style="font-size: small;">In a query if k=-1, the output 2 space separated integers in a new line denoting the number of nymphs in galaxy a, and galaxy b respectively.</span></p>
<p><span style="font-size: small;"><strong>Constraints:</strong></span></p>
<p><span style="font-size: small;">1 &lt;= T &lt;= 10</span></p>
<p><span style="font-size: small;">2 &lt;= n &lt;= 50,000</span></p>
<p><span style="font-size: small;">The galaxies are connected in such a way that there is a unique path from each galaxy to every other galaxy.</span></p>
<p><span style="font-size: small;">2 &lt;= Q &lt;= 50,000</span></p>
<p><span style="font-size: small;">0 &lt;= a,b &lt;= n-1</span></p>
<p><span style="font-size: small;">a and b are differrent</span></p>
<p><span style="font-size: small;">-1 &lt;= k &lt;= 100</span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong>Time Limits: </strong><strong>8</strong>&nbsp;seconds.</span></p>
<p><span style="font-size: small;"><br></span></p>
<h3><span style="font-size: small;">Example</span></h3>
<pre><span style="font-size: small;"><strong>Input:</strong>
1</span></pre>
<pre><span style="font-size: small;">3</span></pre>
<pre><span style="font-size: small;">0 1</span></pre>
<pre><span style="font-size: small;">1 2</span></pre>
<pre><span style="font-size: small;">2</span></pre>
<pre><span style="font-size: small;">1 2 2</span></pre>
<pre><span style="font-size: small;">0 2 -1 </span></pre>
<pre><span style="font-size: small;">
<span style="font-weight: bold;">Output:</span>
</span></pre>
<pre><span style="font-size: small;">0 2</span></pre>
<pre><span style="font-size: small;"><br></span></pre>
<pre><span style="font-size: small;"><strong>Explanation:</strong> The path from 1 to 2 is 1 -&gt; 2. 2 nymphos are thus sent to galaxies 1 and 2. There were 0 nymphos at galaxy 0 initially.</span></pre>