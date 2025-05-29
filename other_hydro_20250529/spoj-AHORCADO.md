<p>The end of the world always has been a subject of controversy thru history, for example, in year 999 and in the 1999. Now there are  persons that believe that the mayan predicted a change in 2012,  specifically in 21st december, 2012, some other speculate that the EoW  will come with certain asteroid crashing onto Earth, or that planetary  aligning has something to do with it....</p>
<p>At ACM(Association of  Catastrophe Mitigation) they are 100% sure that the end might come with a  Zombie Apocalypsis, accordingly they are preparing with a Zombie Detection  Mechanism, that it is some sort of radar. Right now the  mechanism is on beta testing because is having errors identifying  zombies. Sometimes it gives false positives measures. They have asked  you, a wonderful programmer, to make a program that tells them if a  lecture is right or not, basically you will be given two 2-D snapshots  of zombies locations, let's call them the <span style="text-decoration: underline;">previous</span> and the <span style="text-decoration: underline;">present</span> snapshots, the zombies will be represented by a '*', while empty spaces  will be represented by '.', your awesome program must tell if the  present snapshot is a valid one, based on the previous one. A present  snapshot is considered valid if:</p>
<p>1) It has no less zombies than the previous snapshot.</p>
<p>2)  Every zombie in the previous snapshot could have moved only one square  in each of the eight directions, or it is in the same square it was  previously.</p>
<h3>Input</h3>
<p>The first line will have the dimensions of the snapshots, in the form of R C.</p>
<p>2 ¡Ü <strong>R,C </strong>¡Ü 20</p>
<p>Then  R lines of C characters follow, describing the previous snapshot, then  another set of R lines and C characters each line, that belongs to the  present snapshot. The two snapshots are separated by a line with the character 'N'.</p>
<p>The last test case is followed by 0 0.</p>
<p>There will be at most 9 zombies in previous snapshot.</p>
<h3>Output</h3>
<p>For each test case print VALID, if the two snapshots correspond each other, NOT VALID otherwise.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>5 4<br>....<br>....<br>.*..<br>....<br>....<br>N<br>....<br>....<br>..*.<br>....<br>....<br>6 6<br>......<br>.*..*.<br>......<br>......<br>......<br>......<br>N<br>......<br>....*.<br>......<br>....*.<br>......<br>..*...<br>0 0<br><br><strong>Output:</strong><br><br>VALID<br>NOT VALID<br><br></pre>