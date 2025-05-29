<p>Aventuras, Caminhadas e Montanhas (ACM) is a park known around the world for its vast mountain range. Recently, an infrastructure of cable cars has been built so that locomotion throughout the park becomes easier. The cable car stations are distributed in a rectangular network consisting of N rows and M columns, and the fee to go from one station to any of the others is D dollars.</p>
<p>There are also several hiking trails along the park, for those who appreciate walking in natural environments. The trails connect every horizontally or vertically adjacent station (but not diagonally adjacent ones). Alfredo and his family are visiting the park this summer vacation, and they wish to visit all of the stations in the park.</p>
<p>However, they consider the charged fee as overtly high. Therefore, they plan to mix walking on foot with the use of the cable cars. The route may begin on any of the cable car stations. Alfredo does not do a lot of physical exercise, and for that reason he wishes to only walk in downward slopes. The effort of a walk is proportional to the slope of the trail, that is, walking from a station with a height of <strong>H<sub>1</sub></strong> to another with a height of <strong>H<sub>2</sub></strong> represents an effort of (<strong>H<sub>2</sub></strong> – <strong>H<sub>1</sub></strong>) calories.</p>
<p>As there are many possibilities for such routes, Alfredo asked his son João to determine the optimal route. João, in turn, asked his friend in Campinas, who was studying for the ICPC, to determine the minimal cost and effort of a visit to the ACM park.</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of a test case contains three integers <strong>N</strong>, <strong>M</strong>, <strong>D</strong> (1 ≤ <strong>N</strong>, <strong>M</strong>, <strong>D</strong> ≤ 15).</p>
<p>Each of the next <strong>N</strong> lines contains <strong>M</strong> integers. The <strong>i</strong><sup>th</sup> integer in the <strong>j</strong><sup>th</sup> line, <strong>H<sub>ij</sub></strong>, is the height of the <strong>i</strong><sup>th</sup> station on the <strong>j</strong><sup>th</sup> line of the cable<br>car network (<strong>H<sub>ij</sub></strong> ≤ 100). The last test case is followed by one line with three zeros.</p>
<h3>Output</h3>
<p>For each test case, print a line with two integers, separated by spaces. The first corresponds to the minimal cost of the visit to the park, in dollars. The second represents the effort of the route that has minimal cost.</p>
<p>If there is more than one such route, choose the one with the least effort.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2 1<br>1 2<br>4 3<br>3 3 7<br>1 2 1<br>4 5 3<br>1 2 1<br>0 0 0

<strong>Output:</strong>
0 3<br>21 8
</pre>