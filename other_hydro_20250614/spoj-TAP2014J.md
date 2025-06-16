<p><strong>[ The original version of this problem (in Spanish) can be found at <a title="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf" href="http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf">http://dc.uba.ar/events/icpc/download/problems/tap2014-problems.pdf</a> ]</strong></p>
<p>This problem was included in this contest at the last minute, replacing another one that the jury could not fully prepare in time. We will not tell you much about the original problem because we will use it for the contest next year. We will only say that it was called "<em>Playing with lists</em>" because it deals with integer lists. The input for the problem was formed by <strong>L</strong> lists of integers, and its format was:</p>
<p>- a line with an integer <strong>N<sub>1</sub></strong> indicating the amount of numbers in the first list;</p>
<p>- <strong>N<sub>1</sub></strong> lines each representing an integer in the first list;</p>
<p>- a line with an integer <strong>N<sub>2</sub></strong> indicating the amount of numbers in the second list;</p>
<p>- <strong>N<sub>2</sub></strong> lines each representing an integer in the second list;</p>
<p>...&nbsp;</p>
<p>- a line with an integer <strong>N<sub>L</sub></strong> indicating the amount of numbers in the last list;</p>
<p>- <strong>N<sub>L</sub></strong> lines each representing an integer in the last list.</p>
<p>In an unfortunate accident, Joaquin -a member of the jury- erased the first line of each input file (the one which contains <strong>N<sub>1</sub></strong>). We need your help to restore the input files so we can use the problem next year. Given the file without the first line, we ask you to tell us which are the possible values of <strong>N<sub>1</sub></strong> such that, if we add a line with that value at the beginning, the resulting file will be a valid input according to the description given above.</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This problem was included in this contest at the last minute, replacing another one that the jury could not fully prepare in time. We will not tell you much about the original problem because we will use it for the contest next year. We will only say that it was called "Playing with lists" because it deals with integer lists. The input for the problem was formed by L lists of integers, and its format was:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* a line with an integer N_1 indicating the amount of numbers in the first list;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* N_1 lines each representing an integer in the first list;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* a line with an integer N_2 indicating the amount of numbers in the second list;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* N_2 lines each representing an integer in the second list;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">...&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* a line with an integer N_L indicating the amount of numbers in the last list;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">* N_L lines each representing an integer in the last list.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In an unfortunate accident, Joaquin -a member of the jury- erased the first line of each input file (the one which contains N_1). We need your help to restore the input files so we can use the problem next year. Given the file without the first line, we ask you to tell us which are the possible values of N_1 such that, if we add a line with that value at the beginning, the resulting file will be a valid input according to the description given above.</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains an integer <strong>T</strong> (<strong>1 ¡Ü&nbsp;T&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong>) which indicates the number of lines remaining in the input file. Each of the next <strong>T</strong> lines contains an integer <strong>R<sub>i</sub></strong> which represents the number left on the <strong>i</strong>-th line of the input file after the accident (<strong>1&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;R<sub>i</sub>&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;10<sup>5</sup></strong>&nbsp;for <strong>i = 1, 2, ... , T</strong>).&nbsp;</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>Print a line for each possible value of <strong>N<sub>1</sub></strong>. Print all possible answers in increasing order.</p>
<p>&nbsp;</p>
<div>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">5
3
1
2
4
5</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">2
5</span></pre>
</div>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">10
1
2
3
4
5
6
7
8
9
10</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">1
4
10</span><span style="white-space: normal;">
</span></pre>