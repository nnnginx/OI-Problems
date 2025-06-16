<p>An n x n game board is filled with integers, one positive integer per square. The objective is to travel along any legitimate path from the upper left corner to the lower right corner of the board. &nbsp;<br>&nbsp;<br>Rules <br>&nbsp;<br>1.The number in any one square describes how far a step away from that location must be. &nbsp;<br>2.If the step size moves out of the game board, then that step is not allowed. <br>3.All steps must be either to the right or towards the bottom. &nbsp;<br>&nbsp;<br>Note that a 0 is a dead end which prevents any further progress. &nbsp;<br>&nbsp;<br>Consider the 4 x 4 board shown in Figure 1, where the solid circle identifies the start position and the dashed circle identifies the target. Figure 2 shows the three paths from the start to the target, with the irrelevant numbers in each removed.</p>
<h3><img title="fig" src="file://pQ0A9mvC.png" alt="fig" width="618" height="174"></h3>
<h3>Input</h3>
<p>The first line contains the value of n followed by a nxn matrix depicting the board configuration.</p>
<h3>Output</h3>
<p>The output consists of &nbsp;a single integer, which is the number of paths from the upper left corner to the lower right corner.</p>
<h3>Example&nbsp;</h3>
<p>Input:</p>
<p>4&nbsp;<br>2331 <br>1213 <br>1231 <br>3110 <br><br>Output:<br>3</p>
<p>Input:</p>
<p>4&nbsp;<br>3332 <br>1213 <br>1232 <br>2120</p>
<p>Output:</p>
<p>0<br><br>Input:<br><br>5 <br>11101 <br>01111 <br>11111 <br>11101 <br>11101 <br>&nbsp; &nbsp; &nbsp;&nbsp; <br>Output:<br>7</p>