<p>Little Russell and Mr. Fredricksen are embarking in a new journey  with their balloon house. After visiting South America and helping  Kevin, the Snipe, they decided to travel to Warsaw, Poland where new  specimens of birds might be found.<br><br>Their trip is divided into  several parts. Due to pressure levels and wind speed, each part of their  journey requires that their house is equipped with a minimum number of  balloons. As a good boy scout, Russell has already figured out how many  balloons are necessary to go through each of the parts. The problem is  that atmosphere conditions change and Russel is having trouble  determining how many balloons the house should be equipped with to go  through continuous parts of the journey, so they don't have to fill up  more balloons than necessary.<br><br>To help out Russell, you are to develop a program that must deal with the following queries:</p>
<ul>
<li>Russell has added or removed balloons from the house</li>
<li>The minimum number of balloons at certain part has changed</li>
<li>How  many balloons should be added or removed so that the house goes through  continuous parts of the journey with the minimum necessary number of  balloons?</li>
</ul>
<h3>Input</h3>
<p>The first line contains a number <strong>T</strong> (<strong>T</strong> �� 100), the number of testcases.</p>
<p>Each testcase starts with numbers <strong>N</strong> (1 �� N �� 10<sup>5</sup>) and <strong>M</strong> (0 �� M �� 10<sup>3</sup>) where <strong>N</strong> is the number of parts in the journey and <strong>M</strong>&nbsp; is the initial number of balloons in the house. Then <strong>N</strong> numbers follow, one per line, where each number <strong>N<sub>i</sub></strong> (0 �� <strong>N<sub>i</sub></strong> �� 10<sup>9</sup>, 0 �� <strong>i</strong> &lt; <strong>N</strong>) represents the initial number of balloons necessary to go through part <strong>i</strong>.</p>
<p>On the next line there is a number <strong>Q</strong> (1 �� Q �� 10<sup>5</sup>), the number of queries that you should answer. Each of the next <strong>Q</strong> lines contains a query in one of the following formats:</p>
<ul>
<li><em>"<strong>A K</strong></em>" -&nbsp; where <strong>A</strong> is the actual character 'A' (quotes for clarity) and <strong>K</strong> (-10<sup>3</sup> �� <strong>K</strong> �� 10<sup>3</sup>)  is the number of balloons that have been added or removed from the  house.&nbsp; It is assured that the total number of balloons in the house is  never negative;</li>
<li>"<em><strong>B </strong><strong>J </strong><strong>K</strong></em>" - where <strong>B</strong> is the actual character 'B' (quotes for clarity), <strong>J</strong> (0 �� <strong>J</strong> &lt; <strong>N</strong>) is the number of the part of the journey (0-indexed) and <strong>K</strong> (0 �� <strong>K</strong> �� 10<sup>9</sup>) is the new minimum number of balloons required to go through part <strong>J</strong>;</li>
<li><em><strong>"C I J"</strong></em> - where <strong>C</strong> is the actual character 'C' (quotes for clarity), and <em><strong>[I, J]</strong></em>, 0 �� <strong>I</strong> �� <strong>J</strong> &lt; N$ is the range that Russell would like to query. For each query of this type, print the difference between the number of balloons currently in the house and the <strong>minimum</strong> necessary to go through all the parts between <strong>I</strong> and <strong>J</strong> inclusive. Note that this query doesn't change the number of balloons in the house.</li>
</ul>
<h3>Output</h3>
<p>For each testcase print one line with "<em>Testcase X:</em>" (quotes for clarity) where <strong>X</strong> is the number of the testcase (0-indexed). For each query of the type "<em><strong>C I J</strong></em>"  print one line with the difference between the number of balloons  currently in the house and the minimum necessary to go through all the  parts between <strong>I</strong> and <strong>J</strong> inclusive.</p>
<p>Print one blank line after each testcase.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>3 11<br>5 2 4<br>1<br>C 0 2<br>3 11<br>16 2 17<br>5<br>C 0 2<br>A -2<br>C 1 2<br>B 0 0<br>C 0 1

<strong>Output:</strong>
Testcase 0:<br>6<br><br>Testcase 1:<br>6<br>8<br>7
</pre>