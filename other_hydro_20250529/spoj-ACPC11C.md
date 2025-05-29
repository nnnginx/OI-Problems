<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You are visiting circleland, and you have long waited to visit their famous art exhibition.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The exhibition has N rooms arranged in a cycle. In every room, there are some artistic</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">pieces. The rooms are named R1 , R2 , ..., RN . There are also N corridors, named C1 , C2 ,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">..., CN , of lengths L1 , L2 , ..., LN , respectively. Each corridor Ci connects the two rooms Ri</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">and Ri+1 , except CN which connects RN and R1 . Thus, the whole exhibition forms a cycle.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">You can walk in both directions in every corridor.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">There is a single entrance to the exhibition in room R1 , but there are exits in every room.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">As there is nothing interesting to see in the corridors, you would like to spend the least effort</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">walking through corridors in the exhibition. Compute the minimum total distance you need</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">to walk in corridors such that you enter from the entrance, exit from any exit and visit all</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">rooms.</div>
<p>&nbsp;</p>
<p>You are visiting circleland, and you have long waited to visit their famous art exhibition.&nbsp;The exhibition has N rooms arranged in a cycle. In every room, there are some artistic&nbsp;pieces. The rooms are named R1 , R2 , ..., RN . There are also N corridors, named C1 , C2 ,&nbsp;..., CN , of lengths L1 , L2 , ..., LN , respectively. Each corridor Ci connects the two rooms Ri&nbsp;and Ri+1 , except CN which connects RN and R1 . Thus, the whole exhibition forms a cycle.&nbsp;You can walk in both directions in every corridor.&nbsp;</p>
<p>There is a single entrance to the exhibition in room R1 , but there are exits in every room.&nbsp;As there is nothing interesting to see in the corridors, you would like to spend the least effort&nbsp;walking through corridors in the exhibition. Compute the minimum total distance you need&nbsp;to walk in corridors such that you enter from the entrance, exit from any exit and visit all&nbsp;rooms.</p>
<p>&nbsp;</p>
<p style="padding-left: 330px; "><strong><span style="font-size: medium;">&nbsp;Input</span></strong></p>
<p>&nbsp;</p>
<p>Your program will be tested on one or more test cases. The first line of the input will be&nbsp;a single integer T , the number of test cases (1 ¡Ü T ¡Ü 100). Next T lines contain the test&nbsp;cases, each on a single line.&nbsp;</p>
<p>Each case starts with an integer N , the number of rooms in the exhibition (2 ¡Ü N ¡Ü&nbsp;100, 000), followed by N numbers, the lengths of the corridors, L1 , L2 , ..., LN , in this order&nbsp;(1 ¡Ü Li ¡Ü 1,000,000).</p>
<p>The sum of the lengths of all corridors will not exceed 1,000,000,000.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, output, on a single line, a single number representing the minimum total&nbsp;distance you have to walk in corridors such that you visit all rooms.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5 1 1 1 1 1
7 100 15 20 42 33 15 24

<strong>Output:</strong>
4
149</pre>