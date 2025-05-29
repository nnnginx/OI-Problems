<p>As most of you might already know, the Intel-class hi-tech processors of today do a series of parallel tasks to help speedup instruction execution. The most complicated of those tasks is branch prediction. Since the instruction chunks on a modern processor are broken down into independent chunks and executed for a speed up, there is always a requirement to predict what branch an execution path will take (before the actual operands required for the condition to be evaluated to
select the branch, are available). This complex task, is not addressed to fullest level today, but heuristics (as always) have helped.</p>

<p>The task we are going to consider now is much more simple compared to the actual branch prediction task. For our modelling, let us suppose that every instruction has the following syntax: <br>
<current-label> <branched-label><br>
All labels are strings of alphabets only. Labels are case-sensitive.</branched-label></current-label></p>
<p>Moreover the probability that a certain branch will be taken is <strong>P</strong> (it is equal for all branches). If a branch is taken, the point of
execution (control) goes to the branched-label. Otherwise the next statement in that order is executed. Control starts at the "<strong>start</strong>" (lowercase) label and control ends at the "<strong>end</strong>"
(lowercase) label. The branch-label of start and end are themselves, and when start is executed, the control goes to the next instruction, and when end is executed, processing ends, with 100% probability. The last statement in the program is always an ¡°<strong>end</strong>¡±.</p>

<p>It is required to find the expected number of times a statement executes.</p>
<h3>Input</h3>
<p>
  T ¨C the number of test cases;<br>
  For each test case:<br>
  1st line contains one integer N (the number of lines to follow), one real P and one label L.<br>
Each of the N lines that follow consist of instructions (two labels).

</p><h3>Output</h3>
<p>For each test case, output one line containing: <br>
"Expected number of times label L is executed is R",<br>
  where L - is the label given in the input<br>
  R - is the number of times the label is expected to be executed. It must be printed with exactly five decimal places.</p>
<p><strong>Constraints:</strong><br>
  T&lt;=20<br>

  3&lt;=N&lt;=120.<br>
  P lies between 0.01 and 0.99, i.e. no jump is 100% sure.<br>
  Also you can assume no label occurs on the jump side, without being defined throughout the program. <br>
  Each label is less than 10 characters in length.<br>
  Also each line has a distinct label associated with it.</p>

<h3>Example</h3>
<tt>
<p><strong>Sample Input:</strong><br>
  3<br>
  5 .5 B<br>
  C start<br>
  start start<br>
  B C<br>

  D C<br>
  end end<br>
  5 .99 C<br>
  start start<br>
  A B<br>
  B A<br>

  C end<br>
  end end<br>
  3 .5 label<br>
  start start<br>
  label label<br>
  end end</p>

<p><strong>Sample Output:</strong><br>
  Expected number of times label B is executed is 4.00000<br>
  Expected number of times label C is executed is 1.00000<br>
  Expected number of times label label is executed is 2.00000 </p>
</tt>