<p><span style="font-size: small;">It is the Annual Parade of the Galactical Wars. Great men and women from around the cosmos have come to view this spectacular event. To make this a special occasion, the leaders in galaxy H2 have decided to arrange his participants in a particularly beautiful order. </span></p>
<p><span style="font-size: small;">Firstly, they have chosen n particularly suited participants. These n participants have distinct heights ranging from 1 to n. They have arranged them in some way, so that the height of the ith student is H(i).</span></p>
<p><span style="font-size: small;">The sworn enemies of H2, galaxy H3 have obtained some secret information on this arrangement. They know that there is a set of elements A(containing total k indices), such that&nbsp;</span><span style="font-size: small;">H(j) &lt; H(j-1) <strong>IF AND ONLY IF</strong> j belongs to A. As a Martian on H3, your organizer asks you to find the number of such possible configurations that H2 could have made.</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Input:&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">A single line containing space separated integers: n and k</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Next line containing k indices as explained in the problem.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">A single line containing the number of ways to arrange participants modulo 1000000009 ( 10 ^ 9 + 9)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= n &lt;= 700</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= m &lt;= n-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">2 &lt;= i &lt;= n (i is an index)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">All i¡¯s are unique.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Time Limit: 4 seconds.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Examples:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">3 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">There are 2 possible ways to arrange the participants, where their heights are:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">2 1 3 or 3 1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 20px; width: 1px; height: 1px; overflow: hidden;">Note 3 2 1 is not a valid ordering since h(3) &lt; h(2).</div>
<p><strong>Input:</strong>&nbsp;</p>
<p>A single line containing space separated integers: n and k</p>
<p>Next line containing k indices as explained in the problem.</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>A single line containing the number of ways to arrange participants modulo <strong>1000000009</strong> ( 10 ^ 9 + 9)</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= n &lt;= 700</p>
<p>0 &lt;= k &lt;= n-1</p>
<p>2 &lt;= i &lt;= n (i is an index)</p>
<p>All i¡¯s are unique.</p>
<p>&nbsp;</p>
<p>Time Limit: 4 seconds.</p>
<p>&nbsp;</p>
<p><strong>Examples:</strong></p>
<p>&nbsp;</p>
<p><strong>Input:</strong></p>
<p>3 1</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Output:</strong></p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Explanation</strong>: There are 2 possible ways to arrange the participants, where their heights are:</p>
<p>2 1 3 or 3 1 2</p>
<p>&nbsp;</p>
<p>Note 3 2 1 is <strong>not</strong> a valid ordering since h(3) &lt; h(2).</p>
<p>&nbsp;</p>