<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<p><span style="font-style: italic;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Argentina's rugby is currently in one of its best moments of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">all time. Recently the under-18 and under-21 national teams</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">qualified for their corresponding world cups, so the coaches of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">both teams have asked the Incredible Commission for the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Production of Clothing (ICPC) to provide the t-shirts for these</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">events. Each team is formed by N players, but because the two</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">world cups do not take place simultaneously it was agreed that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the ICPC would provide only N t-shirts, to be used by both</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">teams.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For this reason, the t-shirts must be a valid set of clothing</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for both teams. The rules if the rugby world cups state that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">each player must go in the field with a t-shirt imprinted with</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">a unique number, along with a prefix of the player's surname,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">not necessarily unique. This includes boundary cases such as a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">t-shirt with no surname prefix (that is, a prefix of length 0)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and a t-shirt with a complete surname.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The experts of ICPC immediately realized that they could simply</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">provide N t-shirts with only numbers and no surnames on them,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">and each of them would be a valid t-shirt to be used by any</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">player. However, the coaches would rather have the t-shirts</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">with the longest possible prefixes, of course without violating</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">world cup rules, because this way it's easier for them to</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">identify the players while the matches are taking place.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Your task is to help the ICPC finding the maximum amount of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">letters that can be imprinted on a set of N t-shirts, so that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">this set is a valid clothing set for both teams. For example,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">if we have N=3 players, the under-18 team is composed of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"PEREZ", "GONZALEZ" and "LOPEZ", whereas the under-21 team is</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">composed of "GARCIA", "PERALTA" and "RODRIGUEZ", the optimal</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">choice consists in having one t-shirt with the 1-letter prefix</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"G" (to be used by "GONZALEZ" and "GARCIA"), another one with</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">the 3-letter prefix "PER" (to be used by "PEREZ" and</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">"PERALTA"), and the third t-shirt with a 0-letter prefix (to be</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">used by "LOPEZ" and "RODRIGUEZ"). This way, the answer in this</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">case would be 1+3+0=4.</div>
<p>Argentina's rugby is currently in one of its best moments of&nbsp;all time. Recently the under-18 and under-21 national teams&nbsp;qualified for their corresponding world cups, so the coaches of&nbsp;both teams have asked the Incredible Commission for the&nbsp;Production of Clothing (ICPC) to provide the t-shirts for these&nbsp;events. Each team is formed by <strong>N</strong> players, but because the two&nbsp;world cups do not take place simultaneously it was agreed that&nbsp;the ICPC would provide only <strong>N</strong> t-shirts, to be used by both&nbsp;teams.</p>
<p>For this reason, the t-shirts must be a valid set of clothing&nbsp;for both teams. The rules of the rugby world cups state that&nbsp;each player must go in the field with a t-shirt imprinted with&nbsp;a unique number, along with a prefix of the player's surname,&nbsp;not necessarily unique. This includes boundary cases such as a&nbsp;t-shirt with no surname prefix (that is, a prefix of length <strong>0</strong>)&nbsp;and a t-shirt with a complete surname.</p>
<p>The experts of ICPC immediately realized that they could simply&nbsp;provide <strong>N</strong> t-shirts with only numbers and no surnames on them,&nbsp;and each of them would be a valid t-shirt to be used by any&nbsp;player of any of the two teams. However, the coaches would rather have the t-shirts&nbsp;with the longest possible prefixes, of course without violating&nbsp;world cup rules, because this way it's easier for them to&nbsp;identify the players while the matches are taking place.</p>
<p>Your task is to help the ICPC finding the maximum amount of&nbsp;letters that can be imprinted on a set of <strong>N</strong> t-shirts, so that&nbsp;this set is a valid clothing set for both teams. For example,&nbsp;if we have <strong>N = 3</strong> players, the under-18 team is composed of&nbsp;<span style="font-family: 'courier new', courier;">"PEREZ"</span>, <span style="font-family: 'courier new', courier;">"GONZALEZ"</span> and <span style="font-family: 'courier new', courier;">"LOPEZ"</span>, whereas the under-21 team is&nbsp;composed of <span style="font-family: 'courier new', courier;">"GARCIA"</span>, <span style="font-family: 'courier new', courier;">"PERALTA"</span> and <span style="font-family: 'courier new', courier;">"RODRIGUEZ"</span>, the optimal&nbsp;choice consists in having one t-shirt with the <strong>1</strong>-letter prefix&nbsp;<span style="font-family: 'courier new', courier;">"G"</span> (to be used by <span style="font-family: 'courier new', courier;">"GONZALEZ"</span> and <span style="font-family: 'courier new', courier;">"GARCIA"</span>), anotherone with&nbsp;the <strong>3</strong>-letter prefix <span style="font-family: 'courier new', courier;">"PER"</span> (to be used by <span style="font-family: 'courier new', courier;">"PEREZ"</span> and&nbsp;<span style="font-family: 'courier new', courier;">"PERALTA"</span>), and the third t-shirt with a <strong>0</strong>-letter prefix (to be&nbsp;used by <span style="font-family: 'courier new', courier;">"LOPEZ"</span> and <span style="font-family: 'courier new', courier;">"RODRIGUEZ"</span>). This way, the answer in this&nbsp;case would be <strong>1+3+0=4</strong>.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using three lines. The first line&nbsp;contains a single integer number <strong>N</strong>, indicating the number of&nbsp;players in each of the two teams (<strong>1 ��&nbsp;N&nbsp;��&nbsp;10<sup>4</sup></strong>). The second&nbsp;line contains the surnames of the <strong>N</strong> players in the under-18&nbsp;team, whereas the third line contains the surnames of the <strong>N</strong>&nbsp;players in the under-21 team. Each surname is a non-empty&nbsp;string of at most <strong>100</strong> uppercase letters. In each test case&nbsp;the total number of characters in the <strong>2N</strong> surnames is at most&nbsp;<strong>10<sup>5</sup></strong>, and two or more players of the same or different teams&nbsp;may have the same surname.</p>
<p>The end of the input is indicated by a line containing the&nbsp;number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing&nbsp;an integer number, representing the maximum number of letters&nbsp;that can be imprinted on a set of <strong>N</strong> valid t-shirts to be used&nbsp;by both teams as explained in the problem statement.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">3
PEREZ GONZALEZ LOPEZ
GARCIA PERALTA RODRIGUEZ
2
RODRIGO GONZALEZ
GONZALO RODRIGUEZ
3
LOPEZ PEREZ LOPEZ
PEREZ LOPEZ LOPEZ
1
GIMENEZ
JIMENEZ
6
HEIDEGGER GAUSS GROTHENDIECK ERDOS CHURCH TURING
HEISENBERG GALOIS EULER ALLEN GODEL CHURCHILL
-1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">4
12
15
0
13</span><span style="white-space: normal;">
</span></pre>