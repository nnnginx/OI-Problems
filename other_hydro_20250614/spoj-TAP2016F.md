<p><strong>[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at <a href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a> ]</strong></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Fidel has finished a fruitful stage of his academic formation by achieving his PhD in Physics. This was mainly the result of his firm attitude towards the formalization of the fabulous results in his fantastic investigation.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Fidel has always spread happiness among his friends and family, and that is why we have all agreed to sign a congratulation letter addressed to our favourite doctor. Having finished writing the letter, the only remaining task is to include the fervent signature of the F signers. For that purpose, we have bought two markers, one of which is French blue and the other fuchsia. Each of the signers will write their name using these markers.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">It is our intention to emphasize the doctor title that Fidel has just achieved, and so we want that the abbreviation of such title ("DR") can be seen many times disguised within our signatures. To that end, we will sign using both colors, and write some letters in blue and others in fuchsia, in such a way that by reading only the fuchsia letters, Fidel may read the "DR" abbreviation.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">More precisely, our goal is that by reading only those letters written in fuchsia, Fidel only reads 'D' and 'R' letters, in an alternating fashion. Consequently, the first fuchsia letter must be a 'D', and for every 'D' written in fuchsia, the next letter written in that same colour will have to be an 'R'. Similarly, for each 'R' written in fuchsia, the next letter written in that same colour will have to be a 'D', and the very last letter written in fuchsia will have to be an 'R'.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We want to write the fuchsia letters in such a way that Fidel reads the letters 'D' and 'R' written in that colour as many times as possible. In order to accomplish our goal, we can choose in which order we will write our names, and which letters we will write using each colour. Since there are many different ways to do so, we need your help to find out what is the maximum number of times that we can write the "DR" abbreviation in fuchsia, by following the rules that were explained in the previous paragraph.</div>
<p>Fidel has finished a fruitful stage of his academic formation by achieving his PhD in Physics. This was mainly the result of his firm attitude towards the formalization of the fabulous results in his fantastic investigation.</p>
<p>Fidel has always spread happiness among his friends and family, and that is why we have all agreed to sign a congratulation letter addressed to our favourite doctor. Having finished writing the letter, the only remaining task is to include the fervent signature of the <strong>F</strong> signers. For that purpose, we have bought two markers, one of which is French blue and the other fuchsia. Each of the signers will write their name using these markers.</p>
<p>It is our intention to emphasize the doctor title that Fidel has just achieved, and so we want that the abbreviation of such title ("DR") can be seen many times disguised within our signatures. To that end, we will sign using both colors, and write some letters in blue and others in fuchsia, in such a way that by reading only the fuchsia letters, Fidel may read the "DR" abbreviation.</p>
<p>More precisely, our goal is that by reading only those letters written in fuchsia, Fidel only reads '<span style="font-family: &quot;courier new&quot;, courier;"><strong>D</strong></span>' and '<span style="font-family: &quot;courier new&quot;, courier;">R</span>' letters, in an alternating fashion. Consequently, the first fuchsia letter must be a '<strong><span style="font-family: &quot;courier new&quot;, courier;">D</span></strong>', and for every '<strong><span style="font-family: &quot;courier new&quot;, courier;">D</span></strong>' written in fuchsia, the next letter written in that same colour will have to be an '<strong><span style="font-family: &quot;courier new&quot;, courier;">R</span></strong>'. Similarly, for each '<strong><span style="font-family: &quot;courier new&quot;, courier;">R</span></strong>' written in fuchsia, the next letter written in that same colour will have to be a '<strong><span style="font-family: &quot;courier new&quot;, courier;">D</span></strong>', and the very last letter written in fuchsia will have to be an '<strong><span style="font-family: &quot;courier new&quot;, courier;">R</span></strong>'.</p>
<p>We want to write the fuchsia letters in such a way that Fidel reads the letters '<strong><span style="font-family: &quot;courier new&quot;, courier;">D</span></strong>' and '<strong><span style="font-family: &quot;courier new&quot;, courier;">R</span></strong>' written in that colour as many times as possible. In order to accomplish our goal, we can choose in which order we will write our names, and which letters we will write using each colour. Since there are many different ways to do so, we need your help to find out what is the maximum number of times that we can write the "DR" abbreviation in fuchsia, by following the rules that were explained in the previous paragraph.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains an integer <strong>F</strong>, representing the number of signers (<strong>1 ¡Ü&nbsp;F&nbsp;</strong><strong>¡Ü</strong><strong>&nbsp;1000</strong>). Each of the next <strong>F</strong> lines will contain the name of one of Fidel's friends. The name of each friend is formed by no more than <strong>100 </strong>characters from '<strong><span style="font-family: &quot;courier new&quot;, courier;">A</span></strong>' to '<strong><span style="font-family: &quot;courier new&quot;, courier;">Z</span></strong>'.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you must write a single line containing an integer, indicating the maximum number of times that the "DR" abbreviation can appear in fuchsia once we sign our letter, if we follow the rules explained in this problem statement.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">10
RAMIRO
AUGUSTO
JOAQUIN
JACINTO
NICOLAS
ALEJANDRO
DIJKSTRA
KAJITA
MCDONALD
SCHRODINGE
4
DDD
RRR
DRDR
RDRD
12
MELANIE
DAMIAN
RAMIRO
AUGUSTO
JOAQUIN
JACINTO
NICOLAS
ALEJANDRO
DIJKSTRA
KAJITA
MCDONALD
SCHRODINGER
4
ABCEFG
HIJKLM
NOPQST
UVWXYZ</span>

<strong>Output:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">4
5
5
0</span><span style="white-space: normal;">
</span></pre>