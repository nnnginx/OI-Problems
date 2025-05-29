<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Hogwarts School of Witchcraft and Wizardry has a circular lane having N towers numbered 1 to N. Towers i and i+1 are adjacent to each other for 1 ¡Ü i &lt; N and also towers 1 and N are adjacent to each other. Each of these towers has exactly F number of floors, numbered 1,2,3,..,F-1,F from bottom to top. Floors i and i+1 in a tower are adjacent to each other and it takes one second to move between them. It also takes one second to move between floor 1 of a tower and floor 1 of its adjacent tower. Apart from these, there are M bridges designed for a quick escape in case of a Death Eater attack, each of which connects two floors of different towers. Each of these bridges is given as bi fi bj fj t, meaning it takes t seconds to move along this bridge that connects the floor fi of tower bi and the floor fj of tower bj. All ways are bidirectional.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Given (qbi,qfi) and (qbj,qfj), find the minimum time in seconds it takes to reach floor qfj of tower qbj, starting from floor qfi of tower qbi. You have to answer a lot of such queries.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains the number of test cases T. T cases follow. Each test case consists of N F M in the first line. N is the number of towers, F is the number of floors in each tower and M is the number of bridges. M lines follow, each of the form bi fi bj fj t, as mentioned in the problem statement. Next line contains Q, the number of queries and Q lines follow, each of the form qbi qfi qbj qfj.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For each query of the form qbi qfi qbj qfj, output one line denoting the minimum time in seconds it takes to reach the floor qfj of tower qbj, starting from the floor qfi of tower qbi.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 ¡Ü T ¡Ü 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 ¡Ü N, M ¡Ü 100</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 ¡Ü F ¡Ü 1,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 ¡Ü t ¡Ü 1,000,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 ¡Ü Q ¡Ü 100,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 ¡Ü bi, bj, qbi, qbj ¡Ü N</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 ¡Ü fi, fj, qfi, qfj ¡Ü F</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Time Limit : 5s</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Memory Limit : 64 MB</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5 4 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3 2 4 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 3 3 3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 4 5 3 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3 2 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 3 3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 1 3 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 3 4 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 3 4 4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1</div>
<p>Hogwarts School of Witchcraft and Wizardry has a circular lane having N towers numbered 1 to N. Towers i and i+1 are adjacent to each other for 1 ¡Ü i &lt; N and also towers 1 and N are adjacent to each other. Each of these towers has exactly F number of floors, numbered 1,2,3,..,F-1,F from bottom to top. Floors i and i+1 in a tower are adjacent to each other and it takes one second to move between them. It also takes one second to move between floor 1 of a tower and floor 1 of its adjacent tower. Apart from these, there are M bridges designed for a quick escape in case of a Death Eater attack, each of which connects two floors of different towers. Each of these bridges is given as bi fi bj fj t, meaning it takes t seconds to move along this bridge that connects the floor fi of tower bi and the floor fj of tower bj. All ways are bidirectional.</p>
<p>Given (qbi,qfi) and (qbj,qfj), find the minimum time in seconds it takes to reach floor qfj of tower qbj, starting from floor qfi of tower qbi. You have to answer a lot of such queries.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test cases T. T cases follow. Each test case consists of N F M in the first line. N is the number of towers, F is the number of floors in each tower and M is the number of bridges. M lines follow, each of the form bi fi bj fj t, as mentioned in the problem statement. Next line contains Q, the number of queries and Q lines follow, each of the form qbi qfi qbj qfj.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>For each query of the form qbi qfi qbj qfj, output one line denoting the minimum time in seconds it takes to reach the floor qfj of tower qbj, starting from the floor qfi of tower qbi.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 ¡Ü T ¡Ü 3</p>
<p>2 ¡Ü N, M ¡Ü 100</p>
<p>2 ¡Ü F ¡Ü 1,000,000</p>
<p>1 ¡Ü t ¡Ü 1,000,000</p>
<p>1 ¡Ü Q ¡Ü 100,000</p>
<p>1 ¡Ü bi, bj, qbi, qbj ¡Ü N</p>
<p>1 ¡Ü fi, fj, qfi, qfj ¡Ü F</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>1</p>
<p>5 4 3</p>
<p>1 3 2 4 3</p>
<p>2 3 3 3 2</p>
<p>3 4 5 3 1</p>
<p>5</p>
<p>1 3 2 3</p>
<p>1 3 3 2</p>
<p>1 1 3 4</p>
<p>3 3 4 4</p>
<p>4 3 4 4</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>4</p>
<p>5</p>
<p>4</p>
<p>6</p>
<p>1</p>
<p>&nbsp;</p>
<p>&nbsp;</p>