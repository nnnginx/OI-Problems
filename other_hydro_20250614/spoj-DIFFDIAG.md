<p>Daniel enjoys watching TV series. One of his favorite is "Doctor Chaos". In this series the medical genius is saving people by making difficult diagnosis. In his work he employs the differential diagnosis method. Doctor Chaos writes all the symptoms the patient have on the white board and his team tries to find out the disease which explains those symptoms best. Sometimes some symptoms are not caused by the disease itself. Sometimes some symptoms are not revealed yet and are not written on the board. Anyhow the team chooses come candidate-diseases and then runs the tests to identify the right one. Help Doctor Chaos by making a program which find out the diseases that are explaining the set of symptoms the best way. We'll say that the disease explains the set of symptoms the best way if it explains the most symptoms from the set among all known diseases.

</p><h3>Input</h3>
<p>The first line of the input file contains number <b>n</b> - the amount of diseases known to Chaos and his team. Then <b>n</b> lines follow describing each disease. The description of the disease starts with the name of the disease. Then number <b>k</b> follows, that is the amount of different symptoms caused by the disease. Then there go the names of the symptoms separated by spaces. After the description of all the diseases there is number <b>t</b> - the amount of cases to diagnose. After that <b>t</b> lines follow each containing a set of symptoms. Each set starts with the number <b>q</b> - the amount of different symptoms. Then <b>q</b> names of the symptoms follow separated by spaces. The names of all diseases and symptoms consist of only small latin letters and don't exceed 20 characters. Each symptom in each set is explained by at least one disease.

</p><h3>Constraints</h3>
<p>
1 &lt;= <b>n</b> &lt;= 1000<br>
1 &lt;= <b>k</b> &lt;= 10<br>
1 &lt;= <b>t</b> &lt;= 10000<br>
1 &lt;= <b>q</b> &lt;= 10<br>
There are no more than 1000 different symptoms.
</p>

<h3>Output</h3>
<p>For each case to diagnose first print the line "Diagnosis #x:" where <b>x</b> is the case number starting from one. Then list all the diseases which explains the corresponding set of symptoms best. The diseases should be listed one in line and in the same order in which they were given in the input file.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
migraine 2 headache nausea
poisoning 3 nausea stomachache fever
flu 3 fever cough headache
4
1 fever
2 nausea headache
2 nausea cough
4 fever nausea cough headache

<b>Output:</b>
Diagnosis #1:
poisoning
flu
Diagnosis #2:
migraine
Diagnosis #3:
migraine
poisoning
flu
Diagnosis #4:
flu
</pre>