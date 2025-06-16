<h3>  Movie collection</h3>
<!--l. 3-->
<p>Mr.&nbsp;K.&nbsp;I.&nbsp;has a very big movie collection. He has organized his collection in a big stack. Whenever he wants to watch one of the movies, he locates the movie in this stack and removes it carefully, ensuring that the stack doesn¡¯t fall over. After he finishes watching the movie, he places it at the top of the stack. <!--l. 9--></p>
<p>Since the stack of movies is so big, he needs to keep track of the position of each movie. It is sufficient to know for each movie how many movies are placed above it, since, with this information, its position in the stack can be calculated. Each movie is identified by a number printed on the movie box. <!--l. 15--></p>
<p>Your task is to implement a program which will keep track of the position of each movie. In particular, each time Mr.&nbsp;K.&nbsp;I.&nbsp;removes a movie box from the stack, your program should print the number of movies that were placed above it before it was removed. <!--l. 20--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 21-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with two integers <em>m </em>and <em>r </em>(1 ¡Ü <em>m,r </em>¡Ü 100<span style="margin-left:0.3em">&nbsp;000): the number of movies in       the stack and the number of locate requests. </span></li>
<li>one line with <em>r </em>integers <em>a</em><sub>1</sub><em>,</em><em>¡­</em><em>,a</em><sub>r</sub> (1 ¡Ü <em>a</em><sub>i</sub> ¡Ü <em>m</em>) representing the identification numbers       of movies that Mr.&nbsp;K.&nbsp;I.&nbsp;wants to watch.</li>
</ul>
<!--l. 31-->
<p>For simplicity, assume that the initial stack contains the movies with identification numbers 1<em>, </em>2<em>,</em><em>¡­</em><em>,m </em>in increasing order, where the movie box with label 1 is the top-most box.  <!--l. 35--></p>
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 36-->
<p>Per test case:</p>
<ul>
<li>one line with <em>r </em>integers, where the <em>i</em>-th integer gives the number of movie boxes above       the box with label <em>a</em><sub>i</sub>, immediately before this box is removed from the stack.</li>
</ul>
<!--l. 43-->
<p>Note that after each locate request <em>a</em><sub>i</sub>, the movie box with label <em>a</em><sub>i</sub> is placed at the top of the stack. <!--l. 46--></p>
<p>&nbsp;</p>
<h4>Sample in- and output</h4>
<table align="center" id="TBL-1" border="1" cellspacing="5" cellpadding="5" rules="groups">
<colgroup><col id="TBL-1-1"></colgroup><colgroup id="TBL-1-2g"><col id="TBL-1-2"></colgroup>
<tbody>
<tr id="TBL-1-1-" style="vertical-align:baseline;">
<td id="TBL-1-1-1" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Input</span></p>
</td>
<td id="TBL-1-1-2" style="white-space:wrap; text-align:left;"><!--l. 43-->
<p><span>Output</span></p>
</td>
</tr>
<tr id="TBL-1-2-" style="vertical-align:baseline;">
<td id="TBL-1-2-1" style="white-space:wrap; text-align:left;"><!--l. 46-->
<pre>2
3 3
3 1 1
5 3
4 4 5</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>2 1 0
3 0 4</pre>
</td>
</tr>
</tbody>
</table>
<h4>Copyright notice</h4>
<p>
This problem text is copyright by the NWERC 2011 jury. It is
licensed under the Creative Commons Attribution-Share Alike license
version 3.0; The complete license text can be found at:
<a href="http://creativecommons.org/licenses/by-sa/3.0/legalcode">http://creativecommons.org/licenses/by-sa/3.0/legalcode</a>
</p>