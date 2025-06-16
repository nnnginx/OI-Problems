<p>In a small village beyond seven hills and seven seas, Snow White lives together with N dwarves who spend all their time eating and playing League of Legends. Snow White wants to put an end to this, so she has organized gym classes for them.</p>
<p>At the beginning of each class, the dwarves must stand in line, ordered by their height. For the purposes of this task, assume that the dwarves have heights 1, 2, ..., N (each exactly once) and initially all are standing in sorted order with height from 1 to N. Now Snow White play on them by issuing commands of the form:</p>
<p>• 1 X Y -- dwarves with height X and Y in the line must switch places. She also checks their ordering by issuing queries of the form:<br>• 2 A B -- do dwarves with heights A, A+1, ..., B (not necessarily in that order) occupy a contiguous subsequence of the current line? Help the doofus dwarves follow Snow White's instructions and respond to her queries.</p>
<p><strong>INPUT</strong><br>The first line of input contains the two positive integers N and M, the number of dwarves and the number of Snow White's requests, respectively (2 ≤ N ≤ 200 000, 2 ≤ M ≤ 200 000). Each of the following M lines contains a single Snow White's request, of the form "1 X Y" (1 ≤ X, Y ≤ N, X ≠ Y) or “2 A B” (1 ≤ A ≤ B ≤ N), as described in the problem statement.</p>
<p><br><strong>OUTPUT</strong><br>The output must contain one line for each request of type 2, containing the reply to the query, either “YES” or “NO”.</p>
<p>&nbsp;</p>
<p><strong>Example</strong>:</p>
<p><strong>Input</strong> :</p>
<p>4 5<br>2 2 3<br>2 2 4<br>1 1 3<br>2 3 4<br>1 4 3</p>
<p><strong>Output</strong> :</p>
<p>YES</p>
<p>YES</p>
<p>NO</p>