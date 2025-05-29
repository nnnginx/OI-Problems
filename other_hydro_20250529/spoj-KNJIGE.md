<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko has a home library consisting of N books arranged one on top of the other in a narrow cabinet.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Since being well trained in the secrets of alphabet in the previous task, he now wishes to arrange the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">books alphabetically, so that the book whose title comes first alphabetically ends up on top, and the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">alphabetically last one at the bottom of the pile.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko can easily pull a book out of the cabinet, but it is difficult to push it back into the pile, so the</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">book can only be returned to the top of the pile. Thus, the only available method of sorting the books</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">is repeatedly pulling a book out of the pile and placing it on top of the pile.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The books are labelled with integers from 1 to N, in alphabetical order. Therefore, Mirko wants them</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">to be ordered as (1, 2, ..., N), counting from the top. For example, if N = 3 and the starting order is (3,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2, 1), two moves are sufficient. First, he pulls out the book number 2 and places it on top, so the pile</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">becomes (2, 3, 1). After that, he does the same with book number 1, thus the pile becomes (1, 2, 3).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Help Mirko by calculating the minimum number of moves needed to sort a given starting order.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">INPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line of input contains the integer N (N ¡Ü 300 000).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Each of the next N lines contains a single positive integer. These N integers represent the order of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Mirko¡¯s books from top to bottom of the cabinet. Each of the integers 1, 2, ..., N appears exactly once.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">OUTPUT</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first and only line of output must contain the required minimum number of moves.</div>
<p>&nbsp;</p>
<p>Mirko has a home library consisting of N books arranged one on top of the other in a narrow cabinet.&nbsp;Since being well trained in the secrets of alphabet in the previous task, he now wishes to arrange the&nbsp;books alphabetically, so that the book whose title comes first alphabetically ends up on top, and the&nbsp;alphabetically last one at the bottom of the pile.</p>
<p>Mirko can easily pull a book out of the cabinet, but it is difficult to push it back into the pile, so the&nbsp;book can only be returned to the top of the pile. Thus, the only available method of sorting the books</p>
<p>is repeatedly pulling a book out of the pile and placing it on top of the pile.</p>
<p>The books are labelled with integers from 1 to N, in alphabetical order. Therefore, Mirko wants them&nbsp;to be ordered as (1, 2, ..., N), counting from the top.</p>
<p>For example, if N = 3 and the starting order is (3,&nbsp;2, 1), two moves are sufficient. First, he pulls out the book number 2 and places it on top, so the pile&nbsp;becomes (2, 3, 1). After that, he does the same with book number 1, thus the pile becomes (1, 2, 3).</p>
<p>Help Mirko by calculating the minimum number of moves needed to sort a given starting order.</p>
<p>&nbsp;</p>
<p>Input</p>
<p>The first line of input contains the integer N (N ¡Ü 300 000).</p>
<p>Each of the next N lines contains a single positive integer. These N integers represent the order of</p>
<p>Mirko¡¯s books from top to bottom of the cabinet. Each of the integers 1, 2, ..., N appears exactly once.</p>
<p>Output</p>
<p>The first and only line of output must contain the required minimum number of moves.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 
3 
2 
1 

<strong>Output:</strong>
2</pre>