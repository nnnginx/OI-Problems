<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">As a token of thanks for his help, Elizabeth Sinskey has gifted Robert Langdon an amazing set of Russian dolls. The dolls have the property that if doll A has height HA and doll B has height HB, then B can fit inside A if HA&gt;=HB.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Robert noted the heights of the dolls (two dolls can have same height), and then arranged the dolls in a line beautifully. For each doll he noted down the number of dolls that are before this doll in the line and can contain this doll. He wrote this down on another piece of paper.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Accidentally, the dolls fell out of line, and Robert wants to arrange them back beautifully. Given the two pieces of information (heights of the dolls and number of dolls before this in line that can contain this doll), can you rearrange the dolls beautifully?</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line contains T, number of test cases</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case consists of 3 lines</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line of each test case has a single number N, number of dolls.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Second line contains array H, space separated array of size N containing the heights of dolls.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Third line contains array C, space separated array of size N, C[i] indicating number of dolls before this in the beautiful arrangement that can contain doll i.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each test case, output a single line containing the heights of dolls in order as they were when Robert arranged them beautifully.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Assume that a valid solution always exists.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 13 14</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 0 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">12 14 13</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">0 1 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">13 14 12</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">13 12 14</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXPLAINATION:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the first case, (arrangement 13,14,12) 13 and 14 cannot be contained by any doll prior to them, but 12 can be put in doll 13 as well as doll 14, hence the array 0 0 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For the second case, (arrangement 13,12,14) 12 can be contained in 13, hence the array 0 1 0</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CONSTRAINTS:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=T&lt;=500</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=N&lt;=500</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=H[i]&lt;=10^9</div>
<p>As a token of thanks for his help, Elizabeth Sinskey has gifted Robert Langdon an amazing set of Russian dolls. The dolls have the property that if doll A has height H<sub>A</sub> and doll B has height H<sub>B</sub>, then B can fit inside A if H<sub>A</sub>&gt;=H<sub>B</sub>.</p>
<p>Robert noted the heights of the dolls (two dolls can have same height), and then arranged the dolls in a line beautifully. For each doll he noted down the number of dolls that are before this doll in the line and can contain this doll. He wrote this down on another piece of paper.</p>
<p>Accidentally, the dolls fell out of line, and Robert wants to arrange them back beautifully. Given the two pieces of information (heights of the dolls and number of dolls before this in line that can contain this doll), can you rearrange the dolls beautifully?</p>
<p>&nbsp;</p>
<p>INPUT:</p>
<p>First line contains <strong>T</strong>, number of test cases</p>
<p>Each test case consists of 3 lines</p>
<p>First line of each test case has a single number <strong>N</strong>, number of dolls.</p>
<p>Second line contains array <strong>H</strong>, space separated array of size N containing the heights of dolls.</p>
<p>Third line contains array <strong>C</strong>, space separated array of size N, C[i] indicating number of dolls before this in the beautiful arrangement that can contain doll i.</p>
<p>&nbsp;</p>
<p>OUTPUT:</p>
<p>For each test case, output a single line containing the heights of dolls in order as they were when Robert arranged them beautifully.</p>
<p>Assume that a valid solution always exists.</p>
<p>&nbsp;</p>
<p>EXAMPLE INPUT:</p>
<p>2</p>
<p>3</p>
<p>12 13 14</p>
<p>0 0 2</p>
<p>3</p>
<p>12 14 13</p>
<p>0 1 0</p>
<p>&nbsp;</p>
<p>EXAMPLE OUTPUT:</p>
<p>13 14 12</p>
<p>13 12 14</p>
<p>&nbsp;</p>
<p>EXPLAINATION:</p>
<p>For the first case, (arrangement 13,14,12) 13 and 14 cannot be contained by any doll prior to them, but 12 can be put in doll 13 as well as doll 14, hence the array 0 0 2</p>
<p>For the second case, (arrangement 13,12,14) 12 can be contained in 13, hence the array 0 1 0</p>
<p>&nbsp;</p>
<p>CONSTRAINTS:</p>
<p>1&lt;=T&lt;=500</p>
<p>1&lt;=N&lt;=500</p>
<p>1&lt;=H[i]&lt;=10<sup>9</sup></p>
<p>&nbsp;</p>