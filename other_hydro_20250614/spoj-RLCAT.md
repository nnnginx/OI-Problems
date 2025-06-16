<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">With growing popularity of Robert in Harvard, many students have started opting for his course on Symbolism as institute elective course. Class strength has increased to an extent that even with his eidetic memory; Robert is having a hard time remembering faces of the students in his class. This made him switch to using attendance sheet to take attendance of the class.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Imagine N students sitting in a straight row, students are numbered 1 to N. Attendance sheet is first given to student 1, who uses his own pen to sign the sheet. Then he passes the sheet to student 2, and chooses wheather or not to give him the pen too. If student 2 doesn't get a pen from student 1, he will take out his own pen. Student 2, after signing the sheet, will pass the sheet to student 3, and again makes a choice wheather or not to pass the pen. Note that he can even pass the pen that came to him from student 1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">So first student's pen might end up being used by the entire class.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A person becomes annoyed if his pen is used by someone who is not his friend. Each person has a "compatibility value", and two students are friends if the absolute difference of their compatibility values is less than or equal to a given threshold D.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given compatibility values of each student in the class, find the minimum number of students that must take out their pens to sign so that no one gets annoyed.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE : it is not allowed that a person gets a pen from his neighbour, and passes it along without using it (i.e., uses his own pen for his attendance and passes ahead the pen of his neighbour).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line contains T, number of test cases</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case has two lines</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">First line of each test case contains two space separated integers N and D, indicating the number of students in the class and friendship threshold respectively.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Next line contains a space separated array A of N elements, A[i] being the compatibility value of ith student.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For each testcase, output in a single line minimum number of pens that must be taken out so that the whole class is able to mark the attendance and no one gets annoyed.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 1 2 4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 4 7 1 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CONSTRAINTS:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=T&lt;=1000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=N&lt;=300000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=D&lt;=10^9</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sum of all N over all test cases will not exceed 300000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=A[i]&lt;=10^9</div>
<p>With growing popularity of Robert in Harvard, many students have started opting for his course on Symbolism as institute elective course. Class strength has increased to an extent that even with his eidetic memory; Robert is having a hard time remembering faces of the students in his class. This made him switch to using attendance sheet to take attendance of the class.</p>
<p>Imagine <strong>N</strong> students sitting in a straight row, students are numbered 1 to N. Attendance sheet is first given to student 1, who uses his own pen to sign the sheet. Then he passes the sheet to student 2, and chooses wheather or not to give him the pen too. If student 2 doesn't get a pen from student 1, he will take out his own pen. Student 2, after signing the sheet, will pass the sheet to student 3, and again makes a choice wheather or not to pass the pen. Note that he can even pass the pen that came to him from student 1.</p>
<p>So first student's pen might end up being used by the entire class.</p>
<p>A person becomes annoyed if his pen is used by someone who is not his friend. Each person has a "compatibility value", and two students are friends if the absolute difference of their compatibility values is less than or equal to a given threshold <strong>D</strong>.</p>
<p>Given compatibility values of each student in the class, find the minimum number of students that must take out their pens to sign so that no one gets annoyed.</p>
<p>&nbsp;</p>
<p>NOTE : it is not allowed that a person gets a pen from his neighbour, and passes it along without using it (i.e., uses his own pen for his attendance and passes ahead the pen of his neighbour).</p>
<p>&nbsp;</p>
<p>INPUT:</p>
<p>First line contains <strong>T</strong>, number of test cases</p>
<p>Each test case has two lines</p>
<p>First line of each test case contains two space separated integers <strong>N</strong> and <strong>D</strong>, indicating the number of students in the class and friendship threshold respectively.</p>
<p>Next line contains a space separated array A of N elements, A[i] being the compatibility value of ith student.</p>
<p>&nbsp;</p>
<p>OUTPUT:</p>
<p>For each testcase, output in a single line minimum number of pens that must be taken out so that the whole class is able to mark the attendance and no one gets annoyed.</p>
<p>&nbsp;</p>
<p>EXAMPLE INPUT:</p>
<p>2</p>
<p>5 2</p>
<p>3 1 2 4 5</p>
<p>5 3</p>
<p>1 4 7 1 5</p>
<p>&nbsp;</p>
<p>EXAMPLE OUTPUT:</p>
<p>1</p>
<p>2</p>
<p>&nbsp;</p>
<p>CONSTRAINTS:</p>
<p>1&lt;=T&lt;=1000</p>
<p>1&lt;=N&lt;=300000</p>
<p>1&lt;=D&lt;=10<sup>9</sup></p>
<p>Sum of all N over all test cases will not exceed 300000</p>
<p>1&lt;=A[i]&lt;=10<sup>9</sup></p>