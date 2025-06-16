<p>There are <strong>N</strong> schools, with i th school having <strong>S<sub>i</sub></strong> students. There is a inter-school programming contest <strong>IPC</strong> in which all the schools participate. As <strong>IPC</strong> is a very prestigious event, the schools conduct a test run within themselves. They assign a predicted rank for students within the school for all students, based on the rank they got in the test run. Let <strong>P<sub>ij</sub></strong> be the predicted rank of <strong>j</strong> th student of <strong>i</strong> th school. The predicted rank will be unique within the school, i.e. formally:<br> <img title="\fn_jvn \{\forall i, P_i_j = P_i_k \Leftrightarrow j=k\}" src="./22973/file/NfbE3tyk.png" alt=""> <br>It should be noted that students of different schools may have the same predicted rank. <br> <br> At the end of IPC, the IPC committee has given each school the result card containing the marks of all students of that school. Let <strong>M<sub>ij</sub></strong> represent the actual marks obtained by the <strong>j</strong> th student of <strong>i</strong> th school. IPC follows a strict rule of giving unique marks to all students taking part in IPC, i.e. formally:<br> <img title="\fn_jvn \{\forall i, \forall j , M_i_j = M_p_k \Leftrightarrow i=p \and\ j=k\}" src="./22973/file/cxWONSmA.png" alt=""> <br> <br> You are to design a system, which will efficiently answer queries of the following form:<br> <strong>L</strong> - the number of schools to be considered<br> <strong>A1 A2 A3 .... AL</strong> -  the list of schools<br> <strong>P1 P2</strong> - The range of predicted ranks<br> <strong>K</strong> - desired rank<br> You are to answer - among all the students who attended the given list of schools and with predicted ranks between <strong>P1</strong> and <strong>P2</strong> both inclusive, the marks of the student with <strong>K</strong> th highest marks. (The first highest marks would the the maximum marks, and second would be the next and so on)</p>
<p>&nbsp;</p>
<h4>Input</h4>
<p>First line contains a single integer <strong>N</strong>, the number of schools.<br> The next line contains <strong>N</strong> space separated integers <strong>S<sub>i</sub></strong>.<br> The next <strong>N</strong> lines, the <strong>i</strong> th line contains <strong>S<sub>i</sub></strong> space separated integers, <strong>j</strong> th of which is denoting <strong>P<sub>ij</sub></strong>.<br> The next <strong>N</strong> lines, the <strong>i</strong> th line contains <strong>S<sub>i</sub></strong> space separated integers, <strong>j</strong> th of which is  denoting <strong>M<sub>ij</sub></strong>.<br> The next line contains a single integer <strong>Q</strong>, denoting the number of queries.<br> Whats follows are <strong>Q</strong> sets of queries. Each query is structured as follows.<br> First line of the query is <strong>L</strong>, the list of schools.<br> Followed by <strong>L</strong> integers denoting the <strong>1 based</strong> indices of schools.<br> Next are <strong>P1</strong> and <strong>P2</strong>, the range of ranks we are interested in.<br> Next is the integer <strong>K</strong>.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h4>Output</h4>
<p>For each query on a separate line print a single integer answering the query. If answer is not possible print -1</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h4>Constraints</h4>
<p>1 ¡Ü <strong>N</strong> ¡Ü 10 <br> 1 ¡Ü <strong>S<sub>i</sub></strong> ¡Ü 10000 <br> 1 ¡Ü <strong>P<sub>ij</sub></strong> ¡Ü <strong>S<sub>i</sub></strong> <br> 1 ¡Ü <strong>M<sub>ij</sub></strong> ¡Ü 1000000000 <br> 1 ¡Ü <strong>Q<strong> ¡Ü 10000 <br> 1 ¡Ü P1 ¡Ü P2 ¡Ü max(S[i])<br> 1 ¡Ü K ¡Ü sum of all S[i]<br>
</strong></strong></p><p><strong><strong>&nbsp;</strong></strong></p><strong><strong>
<h3>Sample  Input</h3>
<pre>4
1 3 4 1 
1 
1 2 3 
2 3 1 4 
1 
28 
20 11 8 
6 18 22 26 
7 
4
1
2 
3 3
1
1
2 
3 3
1
3
1 3 4 
4 4
1
4
1 2 3 4 
4 4
4
</pre>
<h3>Sample Output</h3>
<pre>8
8
26
-1
</pre>
</strong></strong><p></p>