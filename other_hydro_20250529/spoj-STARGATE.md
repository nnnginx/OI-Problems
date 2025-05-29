<p>   </p>
<table class="problems" style="width: 666px; height: 15px;" border="0">
<tbody>
<tr class="navigation">
<td style="text-align: center;" width="50%"><a href="/problems/STARGATE/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/STARGATE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p><br>
</p><p>"A Long Time Ago, in a Galaxy Far, Far Away..." one advanced civilization discovered a manner of instant traveling between  solar  systems. Since  that moment,  they have  devoted all  their efforts  to  constructing pairs of stargates that connect distant planets. Soon enough communication network became so complex that they require help to maintain information about the connected worlds.</p>
<p>Write a program  that will help  them maintain  information about the connected systems and we will make sure that the best of your solutions will be forwarded to their space-time continuum.</p>
<p>Planets A and B are connected if there is a direct stargate connection between them, or there is a planet sequence  P1,  P2,..Pn where  P1=A,  Pn=B and  there  is  a  direct stargate  connection  between  Pk  and  Pk-1, k ﹋ {2,..n}.</p>
<p>Connections are bidirectional. There can be multiple connection paths between two planets.</p>
<pre><br><h1 style="text-align: center;">Input</h1></pre>
<p>Input file consist of multiple data sets. Each data set occupies one or more lines. There are no empty lines in the input file. Each  line starts with a single letter ＆D＊, ＆C＊ or ＆Q＊ (upper or lower case) followed by 1 to 5 integers with following meaning:</p>
<ul>
<li>＆D＊ (define) has only one argument which defines number of planets N considered in following data set (N&lt;=6000000, planets are numerated from 1..N).</li>
</ul>
<ul>
<li>＆C＊ (connect) creates a connection between a given pair(s) of planets. </li>
<li>＆Q＊ (query) examines if a given pair(s) of planets are connected. </li>
</ul>
<p>Both ＆C＊ and ＆Q＊ command (＆X＊ in following text) share the same syntax:</p>
<p>X src dst 每 Creates a connection (or query) between given pair of planets (src, dst).</p>
<p>X src dst nnn 每 Creates a connection (or query) between src planet and nnn consecutive planets numerated from dst.</p>
<p>Example: C 1 100 3 creates following links (1,100), (1,101), (1,102).</p>
<p>X  src  dst  nnn  step  每  Creates  a  connection  (or  query)  between  src planet  and  nnn  planets numerated from dst with given step.</p>
<p>Example: C 1 100 3 5 creates following links (1,100), (1,105), (1,110).</p>
<p>X src dst nnn dststep srcstep 每 Creates a connection  (or query) between nnn pairs of planets numerated from src with srcstep and dst with dststep respectively.</p>
<p>Example: C 1 100 3 5 15 creates following links (1,100), (16,105), (31,110).</p>
<h3>Output</h3>
<pre><p>Output  file  contains one  line pre each query  (＆Q＊)  line  in  the  input  file.  Each  line  contains two  numbers </p><p>separated by a space. First value represents number of connected planet pairs from appropriate query while second</p><p>represents number of disconnected planet pairs. </p><br><h3>Sample</h3><br><pre>Sample input: <br>d 5 <br>C 1 3 <br>D 20 <br>q 1 3 <br>c 1 10 10 <br>Q 1 2 18 1 1 <br><br>Sample output: <br>0 1 <br>9 9  <br><br>Sample input 1:<br>d 5<br>d 1<br>q 1 1<br>d 10<br>q 1 6 5 1 1<br>c 1 2 9<br>q 1 6 5 1 1<br>Sample output 1:<br>1  0<br>0  5<br>5  0<br></pre>
<br><br><br><br><br><br><strong>Notice : ＆D＊, ＆C＊ or ＆Q＊ can be upper or lower case</strong><br><br></pre>