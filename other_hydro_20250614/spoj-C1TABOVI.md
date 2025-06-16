<p>Zvonkec is yet another programmer employed in a small company. Every day he has to refactor one file of source code. Much to his dismay, the source is usually far from being clear and tidy. He is especially bothered by uneven indentation, i.e. the number of tabulators (tabs) indenting each line.</p>
<p>Fortunately, his editor has a command to select a group of consecutive lines and add or delete a character from the start of each one. Help&nbsp; Zvonkec tidy up the code as quickly as possible.</p>
<p>You are given the number of lines N, a sequence specifying the current number of tabs at the start of each line, and a sequence specifying the required number of tabs at the start of each line.</p>
<p>Zvonkec can execute any number of commands consisting of:</p>
<p>¡ñ selecting any number of consecutive lines<br>¡ñ adding or deleting a single tab to/from the front of each of the selected lines</p>
<p>The two actions above comprise a single command, regardless of the number of selected lines. It should be noted that it is forbidden to delete more tabs from a line than are actually present at the start of a line, as the editor would start deleting characters other than tabs.</p>
<p>You are asked to calculate the minimum number of commands required to tidy up the code.</p>
<h3>Input</h3>
<p>The first line of input contains a positive integer N (N ¡Ü 1000).</p>
<p>The second line contains a sequence of N integers Pi (0 ¡Ü Pi ¡Ü 80), specifying the number of tabs at the start of i-th line before any editing.</p>
<p>The third line contains a sequence of N integers Ki (0 ¡Ü Ki ¡Ü 80), specifying the number of tabs that Zvonkec would like at the start of i-th line.</p>
<h3>Output</h3>
<p>The first and only line of output must contain the required number, as specified in the problem statement.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>3 <br>3 4 5 <br>6 7 8<br><br><strong>Output:</strong><br>3<strong><br><br>Input:</strong><br>4 <br>1 2 3 4 <br>3 1 1 0<strong><br><br>Output:</strong><br>6<strong><br></strong><strong><br>Input:</strong><br>4<br>5 4 5 5<br>1 5 0 1<strong><br><br>Output:</strong><br>10<strong><br></strong><br></pre>