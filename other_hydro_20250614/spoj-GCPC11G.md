<p>The manager of a large security company has to build a new surveillance system for different sites. A site consists of <em>N</em> objects where each object has its own security circle. At the border of the surveillance system a high voltage fence has to be installed. The security zone inside of the fence has to be connected. Furthermore, all objects and their security circles should be inside the security zone. The security circles of different objects will never overlap or touch. Now the manager needs your help. He asks you for the minimal needed fence length.</p>
<p style="text-align: center;"><img src="../../../content/ak15:security1.png" alt="example image" width="40%"> <img src="../../../content/ak15:security2.png" alt="example image" width="40%"></p>
<h3>Input</h3>
<p>The first line of the input gives the number of test cases <em>C</em> (<em>0 ¡Ü C ¡Ü 100</em>). The first line of each such test case holds the integer <em>N</em>: the number of objects in the current site (<em>0 &lt; N ¡Ü 25</em>). Each of the following <em>N</em> lines holds three integers <em>x<sub>i</sub></em>, <em>y<sub>i</sub></em>, and <em>r<sub>i</sub></em> that describe an object. The coordinates of the i-th object and the radius for the needed security circle for this object. (|<em>x<sub>i</sub></em>|,|<em>y<sub>i</sub></em>| ¡Ü <em>100</em>, <em>0 &lt; r<sub>i</sub> ¡Ü 100</em>) (The center of the security circle around an object is the position of the object itself.)</p>
<h3>Output</h3>
<p>For each test case print one line containing the minimal fence length for this case. Your output should have an absolute or relative error of at most <em>10<sup>-7</sup></em>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3
2 2 1
8 2 1
5 6 1
2
6 4 2
2 4 1
4
2 2 2
6 1 1
5 5 2
1 6 1

<strong>Output:</strong>
22.2831853072
17.6761051635
25.4247779608
</pre>