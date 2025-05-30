<p>
In a far away nation, all the liquid substance are stored in a can of shape of a triangular prism. According to belief, this will bring security to their children. As they are very resource conservative people, unlike the earth natives, they want to use as less as possible amount of the raw material to be used for producing the can, which directly depends on the surface area of the can. Mr. Buzz Light Year, of Star Command, is provided with the responsiblity to find the minimal suface area required to prodce a can of a given volume.</p>

<p><strong>Notes:</strong></p>
<ul>
  <li>Consider the material the can is made of to be infinitely thin.</li>
  <li>The base of the prism is equilateral triangle.</li>
  <li>Some formulas:
     <ul>
     <li>a: triangle side's length.</li>
     <li>h: height of the prism.</li>
     <li>Volume, V =&nbsp; (a<sup>2</sup> * sin(60��) * h)/2</li>
     <li>Surface Area, S = a<sup>2</sup>*sin(60��) + 3*a*h</li>
     </ul>
  </li>
  <li>If not provided by a library, use the alue of 2*acos(0) for PI(��).</li>
  <li>Reminder:
    <ul>
    <li>If your result is <b>within 10<sup>-2</sup></b> of the expected result, your solution will be evaluated as correct.</li>
    <li>If your result is <b>between (1-10<sup>-2</sup>)*expected and (1+10<sup>-2</sup>)*expected</b>, it will be evaluated as correct.</li>
    </ul>
   </li>
</ul>
<p><img title="Prism" src="./23970/file/ndMCN0c1.png" alt="Prism" width="265" height="131"></p>

<h3>Constraints</h3>
<p>Given volume will be an integer between 1 and 100000, inclusive.</p>

<h3>Input</h3>
<p>Input begins with a integer t, number of test cases. Then follows t lines, each one containing an integer, V, given volume.</p>

<h3>Output</h3>
<p>For each volume, print the minimum surface area required to produce the can in separate line.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5
10
5
100
245
5421

<strong>Output:</strong>
30.3872837089
19.1427891970
141.0452767471
256.3318686611
2020.2796324002</pre>

<p><b>Explanation for test case 1:</b><br>
Volume = 10, a = 3.41995,  h = 1.97451, Minimum Surface Area = 30.3872837089
</p>