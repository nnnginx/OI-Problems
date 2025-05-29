<h3>  Smoking gun</h3>
<!--l. 3-->
<p>Andy: ¡±Billy the Kid fired first!¡± <br> <!--l. 5--></p>
<p>Larry: ¡±No, I¡¯m sure I heard the first shot coming from John!¡± <br> <!--l. 8--></p>
<p>The arguments went back and forth during the trial after the big shoot-down, somewhere in the old wild west. Miraculously, everybody had survived (although there were serious injuries), but nobody could agree about the exact sequence of shots that had been fired. It was known that everybody had fired at most one shot, but everything had happened very fast. Determining the precise order of the shots was important for assigning guilt and penalties. <!--l. 17--></p>
<p>But then the sheriff, Willy the Wise, interrupted: ¡±Look, I¡¯ve got a satellite image from the time of the shooting, showing exactly where everybody was located. As it turns out, Larry was located much closer to John than to Billy the Kid, while Andy was located just slightly closer to John than to Billy the Kid. Thus, because sound travels with a finite speed of 340 meters per second, Larry may have heard John¡¯s shot first, even if Billy the Kid fired first. But, although Andy was closer to John than to Billy the Kid, he heard Billy the Kid¡¯s shot first ¨C so we know for a fact that Billy the Kid was the one who fired first! <!--l. 28--></p>
<p>Your task is to write a program to deduce the exact sequence of shots fired in situations like the above. <!--l. 31--></p>
<p>&nbsp;</p>
<h4>Input</h4>
<!--l. 32-->
<p>On the first line a positive integer: the number of test cases, at most 100. After that per test case:</p>
<ul>
<li>one line with two integers <em>n </em>(2 ¡Ü <em>n </em>¡Ü 100) and <em>m </em>(1 ¡Ü <em>m </em>¡Ü 1<span style="margin-left:0.3em">&nbsp;000): the number of       people involved and the number of observations. </span></li>
<li><em>n </em>lines with a string <em>S</em>, consisting of up to 20 lower and upper case letters, and two       integers <em>x </em>and <em>y </em>(0 ¡Ü <em>x,y </em>¡Ü 1<span style="margin-left:0.3em">&nbsp;000<span style="margin-left:0.3em">&nbsp;000): the unique identifier for a person and his/her       position in Cartesian coordinates, in metres from the origin. </span></span></li>
<li><em>m </em>lines of the form ¡°<tt>S1</tt><tt>&nbsp;heard</tt><tt>&nbsp;S2</tt><tt>&nbsp;firing</tt><tt>&nbsp;before</tt><tt>&nbsp;S3</tt>¡±, where <em>S</em>1, <em>S</em>2 and <em>S</em>3 are       identifiers among the people involved, and <em>S</em>2<em>¡Ù</em><em>S</em>3.</li>
</ul>
<!--l. 48-->
<p>If a person was never mentioned as <em>S</em>2 or <em>S</em>3, then it can be assumed that this person never fired, and only acted as a witness. No two persons are located in the same position. <!--l. 52--></p>
<p>The test cases are constructed so that an error of less than 10<sup>-7</sup> in one distance calculation will not affect the output. <!--l. 55--></p>
<p>&nbsp;</p>
<h4>Output</h4>
<!--l. 56-->
<p>Per test case:</p>
<ul>
<li>one  line  with  the  ordering  of  the  shooters  that  is  compatible  with  all  of  the       observations, formatted as the identifiers separated by single spaces.</li>
</ul>
<!--l. 63-->
<p>If multiple distinct orderings are possible, output ¡°<tt>UNKNOWN</tt>¡± instead. If no ordering is compatible with the observations, output ¡°<tt>IMPOSSIBLE</tt>¡± instead. <!--l. 67--></p>
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
<pre>3
4 2
BillyTheKid 0 0
Andy 10 0
John 19 0
Larry 20 0
Andy heard BillyTheKid firing before John
Larry heard John firing before BillyTheKid
2 2
Andy 0 0
Beate 0 1
Andy heard Beate firing before Andy
Beate heard Andy firing before Beate
3 1
Andy 0 0
Beate 0 1
Charles 1 3
Beate heard Andy firing before Charles</pre>
</td>
<td id="TBL-1-2-2" style="white-space:wrap; text-align:left;"><!--l. 50-->
<pre>BillyTheKid John
IMPOSSIBLE
UNKNOWN</pre>
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