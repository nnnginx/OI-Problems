<p style="TEXT-ALIGN: justify">The Red Cross is a humanitarian and neutral organization that strives to provide assistance to victims of civil wars and other situations of serious violence.</p>
<p style="TEXT-ALIGN: justify">Recently, Nlogônia entered into a political crisis that culminated in a great civil war. This war wrecked Dozens of innocent communities across the country. Seeing the calamity situation in which the country joined, the Red Cross decided to help the population in all affected regions in Nlogônia.</p>
<p style="TEXT-ALIGN: justify">For this, it was decided that a hospital base will be installed to support the Red Cross in the country. However, the summit do not know where to build the base of Red Cross hospital. You and your team were hired to tell the Red Cross the position that they must build the hospital, with the constraint that the distance to the farthest community from the hospital is as small as possible.</p>
<h3>Input</h3>
<p style="TEXT-ALIGN: justify">The input file consists of several test cases. For each test case, the first line contains the number of affected communities N to be served. Each of the following N lines contains a localization of each community. Localization is represented by decimal coordinates X and Y. After the first test case will be another line with a new test case defined by number of communities N. The input never contains repeated coordinates for each community in each test case and the input ends with N=0.</p>
<p style="TEXT-ALIGN: justify">Suppose:<br>0&lt;=N&lt;=100000<br>(-100000,-100000)&lt;=X,Y&lt;=(100000, 100000)</p>
<h3>Output</h3>
<p>For each test case of your program prints just a one line with two decimal number separated by<br>commas indicating the optimum location for the construction of the base hospital, regardless of the<br>area have a built space. Each coordinate must be printed with four decimal place of accuracy.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>-1 0<br>1 0<br>4<br>0.5&nbsp; 0.5<br>0.5 -0.5<br>0.0&nbsp; 0.5<br>0.0 -0.5<br>0</pre>
<pre><strong>Output:</strong>
0.0000, 0.0000<br>0.2500, 0.0000</pre>