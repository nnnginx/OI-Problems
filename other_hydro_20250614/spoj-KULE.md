<p></p>
<table class="problems" style="width: 99%;" border="0">
<tbody>
<tr class="navigation">
<td><a href="/problems/KULE/english/">English version</a></td>
<td><a href="/problems/KULE/polski/">Wersja polska</a></td>
</tr>
</tbody>
</table>
<p><span style="line-height: normal"> 
</span></p><p>John has a certain number of spheres. Almost all of them have identical weight apart from one. There are a lot of them and John cannot say which one differs from the other ones by himself. You can help him to determine which sphere it is by using the pair of scales.</p>
<h3>Input/Output</h3>
<p>In the first line of the input there is one integer <em><strong>n</strong></em> [3 &lt;= <em><strong>n</strong></em> &lt;= 100 000] that stands for the number of spheres which John has. The spheres are numbered from 1 to <em><strong>n</strong></em>.</p>
<p>You can give John two types of orders (just print them to standard output):</p>
<ul>
<li><strong>WEIGHT<em> m a<sub>1</sub> a<sub>2</sub> ... a<sub>m</sub> b<sub>1</sub> b<sub>2</sub> ... b<sub>m</sub></em></strong>
<p>Weighting spheres. All numbers should be separated with a space and they stand for: <strong>m</strong> - number of spheres that should be put on one of the scales (there should be the same amount of spheres on both of the scales), <strong><em>a<sub>1</sub> a<sub>2</sub> ... a<sub>m </sub></em></strong> - identifiers of spheres that you want John to put on the left scale and <strong><em>b<sub>1</sub> b<sub>2</sub> ... b<sub>m - </sub></em></strong>identifiers of spheres that you want John to put on the right scale.</p>
<p>After conducting the weighting John will tell you about the outcome (which you will be able to read from the standard input). Possible answers are <strong>LEFT</strong> - spheres on the left scale are heavier, <strong>RIGHT</strong> - spheres on the right answer are heavier, <strong>EQUAL</strong> - spheres on both scales have equal weight.</p>
<p>After conducting the weighting John is ready right away to execute the next order.</p>
<p>However, you should remember that if the weighting's number is too high John can become quite bored...</p>
</li>
<li><strong>ANSWER k</strong>
<p>Answering. This order is to give information that <strong>k</strong> is the identifier of the searched sphere; however if the sphere we are looking for is lighter than the other ones you should precede that with a '-' sign.</p>
<p>John no longer needs you after that command (your program should end).</p>
</li>
</ul>
<h3>Example</h3>
<pre>John: 3
You:  WEIGHT 1 1 2
John: LEFT
You:  WEIGHT 1 1 3
John: EQUAL
You:  ANSWER -2
</pre>
<p><strong>Remark: </strong>Program should clear the output buffer after printing each line. It can be done using fflush(stdout) command or you can set the proper type of buffering at the beginning of the execution - setlinebuf(stdout).</p>
 <p></p>