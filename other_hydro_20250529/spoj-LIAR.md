<p>Professor Millman hates us, and worse, characterizes us as liars. We don＊t care if he means it or not, but we (more professional that him!) planned to give the lower and upper bound on the number of liars in the class (so that you know what happens the next time he scolds us! ).</p>
<p>To start with we took a survey of all students in the class. Each student gave a reply about every student saying whether that student is a liar or not. These answers are in the form of a Matrix A, where A[i][j] represents the reply given by the i-th student about the j-th student. If that character is ＆L＊ 每 it means he/she is a liar; if it＊s ＆T＊ 每 then it means that, that student is a truth speaker.</p>
<p>We take the following as our definition of the terms Truth-Speaker, and Liar:<br> Truth-Speaker (＆T＊): All his/her replies are true.<br> Liar (＆L＊) : (S)he has made at least one false reply.</p>
<h3>Input</h3>
<p>T 每 the number of test cases; For each test case :<br> N 每 total number of students in the class<br> Matrix A of NxN characters, without space separation;</p>
<h3>Output</h3>
<p>For i-th test case output one line of the form ※Class Room#i contains atleast A and atmost B liars§, where A and B are the lower and the upper bounds on the number of liars respectively. If there is a paradoxical class room, instead of the above line, print ※Class Room#i is paradoxical§.</p>
<p><strong>Constraints:</strong><br> T&lt;=50; Our class rooms contain atmost 70 students.</p>
<h3>Example</h3>
<p><tt> </tt></p>
<p><tt><strong>Sample Input:</strong><br> 4<br> 2<br> LL<br> TT<br> 3<br> TTT<br> TTT<br> TTT<br> 4<br> TLLL<br> LTLL<br> LLTL<br> LLLT<br> 5<br> TLTLT<br> TTTTT<br> LLTLL<br> LLLLL<br> TLTLT</tt></p>
<p><tt>
</tt></p><p><tt><strong>Sample Output:</strong><br> Class Room#1 is paradoxical<br> Class Room#2 contains atleast 0 and atmost 3 liars<br> Class Room#3 contains atleast 3 and atmost 4 liars<br> Class Room#4 contains atleast 4 and atmost 4 liars</tt></p><tt>
</tt><p></p>
<p>&nbsp;</p>
<p>Here a paradox occurs if a person can't be classified as a liar or a truth-speaker.</p>