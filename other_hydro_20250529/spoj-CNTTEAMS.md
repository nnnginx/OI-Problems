<p>The teacher in the Dystopian School for Politics and other Dirty Games (DSPDG) is training students in group activities. She feels that to really understand group behavior, students need to practice working in groups of different sizes. This is how she groups the students:</p>
<p>There are N students in the class, with roll numbers from 1 to N(2¡ÜN¡Ü10<sup>12</sup>). The teacher generates using her laptop a random permutation of the roll numbers. The student with the roll number equal to the i<sup>th</sup> number in the permutation is assigned as a "target" to the student with roll number as i (Note that "targetship" is not mutual. If 1 is the target for 2, 2 need not be the target for 1). If any student is assigned himself as the target, the teacher generates another permutation till no student is assigned himself.</p>
<p>The N students stand far from each other. Now student 1 goes and joins his target. After this, student 2 (and any student who is with him) joins 2's target. At the i<sup>th</sup> step, student i and anyone who is already with him joins i's target. In case i's target is already with him, nothing is done.</p>
<p>By following this procedure, when all students have joined their targets, the class gets split into some groups. For example, assume that there are 6 students in the class and the permutation that has been generated is {2,4,5,6,3,1}. First, 1 goes and joins 2. Then 1 and 2 join 4. Then 3 joins 5. Then 1, 2 and 4 join 6. 5 is already with 3 and hence does not move. Similarly 6 is already with 1 and does not move. In the end, we have 2 teams : {1,2,4,6} and {3,5}</p>
<p>Given N, find out the expectation value of the number of teams that will be formed when the teacher groups the class in this fashion.</p>
<h3>Input</h3>
<p>First line of the input contains T(¡Ü100), the number of test cases. Following this are T lines, each containing an integer N(2¡ÜN¡Ü10<sup>12</sup>).</p>
<h3>Output</h3>
<p>For each N, output the expectation value of the number of groups formed. Output 6 digits after the decimal point while printing the expectation value</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3
4

<strong>Output:</strong>
1.000000
1.333333
</pre>