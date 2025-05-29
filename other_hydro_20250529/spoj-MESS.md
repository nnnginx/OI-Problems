<p style="text-align: justify;">For the fall semester 2010, EPFL proudly welcomed 2��300 new students to the campus. Handling their registrations to the different sections and levels requires an administrative masterstroke. Nowadays this process is highly automated and worked impeccably up to this year...</p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: center;"><img src="./23368/file/ouxHKWqm.png" alt="" width="381" height="255"></p>
<p style="text-align: justify;">&nbsp;</p>
<p style="text-align: justify;">The software that handles the registrations wasn��t lead out for such a huge number of new students and the secretaries were close to a heart attack when they received the registration printouts. Instead of receiving one sheet per class (defined by the orientation of studies and the level, e.g. Architecture, Bachelor 1) containing the list of all the students registered to that class, the printouts contained sentences in 5 different formats:</p>
<ul>
<li>! <em>STUDENT_ID1</em> studies <em>SECTION</em></li>
<li>! <em>STUDENT_ID1</em> enters semester <em>SEMESTER</em></li>
<li>! <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> chose the same studies</li>
<li>! <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> are in same semester</li>
<li>! <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> are in same class</li>
</ul>
<p style="text-align: justify;"><em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> are the 6-digit sciper numbers, <em>SEMESTER</em> is an integer number in the range from 1 to 10 and <em>SECTION</em> is a one-worded string.</p>
<p style="text-align: justify;">The secretaries were very puzzled and couldn��t figure out how to recreate the expected lists from these printouts. But luckily they remembered PolyProg. The desperate secretaries provide you with the printouts and you are to answer their impatient questions to your best.</p>
<ul>
<li>? What does<em> STUDENT_ID1</em> study</li>
<li>? Which semester will<em> STUDENT_ID1 </em>enter</li>
<li>? Are <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> classmates</li>
</ul>
<p style="text-align: justify;">Two students are considered to be classmates if and only if they study the same subject and enter the same semester. Answering to your best means that your answer must be as complete as possible, you must never give an erroneous answer, but you can just admit that the input was insufficient to answer a question at the point in time it was asked.</p>
<p>Your answers shall respect the following priority:</p>
<table style="width: 621px;" border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="168" valign="top">
<p><strong>Question</strong></p>
</td>
<td width="454" valign="top">
<p><strong>Answer</strong></p>
</td>
</tr>
<tr>
<td width="168" valign="top">
<p>? What   does<em> STUDENT_ID1</em> study</p>
</td>
<td width="454" valign="top">
<p><em>STUDENT_ID1 </em>studies <em>SECTION</em></p>
<p>Sorry,   I have no clue yet</p>
<p>&nbsp;</p>
</td>
</tr>
<tr>
<td width="168" valign="top">
<p>? Which   semester will<em> STUDENT_ID1 </em>enter</p>
</td>
<td width="454" valign="top">
<p><em>STUDENT_ID1 </em>enters semester <em>SEMESTER</em></p>
<p>Sorry,   I have no clue yet</p>
</td>
</tr>
<tr>
<td width="168" valign="top">
<p>? Are   <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> classmates</p>
<p>&nbsp;</p>
</td>
<td width="454" valign="top">
<p>Yes,   <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> are classmates</p>
<p>No,   this is not possible</p>
<p>Possible,   given that <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> study the same subject</p>
<p>Possible,   given that <em>STUDENT_ID1</em> and <em>STUDENT_ID2</em> are in the same semester</p>
<p>Sorry,   I have no clue yet</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p style="text-align: justify;">The input consists of a single test-case with no more than 1��000 printout sentences and no more than 500 questions. They may be mixed and you are to go through them in sequential order, which means that in order to answer a question, you must not rely on any information further down the list. You may safely assume that the sentences are not contradictory! Input terminates on a line containing the single word END.</p>
<p style="text-align: justify;">&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>Output your answers, one per line and terminate with a newline. Be aware of typos :)</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p><span style="font-family: courier new,courier;">! 166554 and 175129 chose the same studies</span></p>
<p><span style="font-family: courier new,courier;">! 175129 and 170113 are in same semester</span></p>
<p><span style="font-family: courier new,courier;">! 166554 studies electronics</span></p>
<p><span style="font-family: courier new,courier;">! 169983 and 170113 chose the same studies</span></p>
<p><span style="font-family: courier new,courier;">? Are 170113 and 169983 classmates</span></p>
<p><span style="font-family: courier new,courier;">! 169983 enters semester 9</span></p>
<p><span style="font-family: courier new,courier;">! 175129 and 169983 are in same semester</span></p>
<p><span style="font-family: courier new,courier;">? Which semester will 170113 enter</span></p>
<p><span style="font-family: courier new,courier;">? Are 169983 and 170113 classmates</span></p>
<p><span style="font-family: courier new,courier;">? Which semester will 166554 enter</span></p>
<p><span style="font-family: courier new,courier;">? What does 175129 study</span></p>
<p><span style="font-family: courier new,courier;">! 169983 studies communicationsystems</span></p>
<p><span style="font-family: courier new,courier;">? Are 166554 and 169983 classmate</span></p>
<p><span style="font-family: courier new,courier;">END</span></p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p><span style="font-family: courier new,courier;">Possible, given that 170113 and 169983 study the same subject</span></p>
<p><span style="font-family: courier new,courier;">170113 enters semester 9</span></p>
<p><span style="font-family: courier new,courier;">Yes, 169983 and 170113 are classmates</span></p>
<p><span style="font-family: courier new,courier;">Sorry, I have no clue yet</span></p>
<p><span style="font-family: courier new,courier;">175129 studies electronics</span></p>
<p><span style="font-family: courier new,courier;">No, this is not possible</span></p>