<p><span style="font-weight: bold;">[Due to SPOJ restrictions, this problem has been modified with respect to the original version used in the Argentinian Programming Tournament of 2016 in order to have multiple test cases per input file. The original version of this problem (in Spanish) can be found at </span><a style="font-weight: bold;" href="http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf">http://torneoprogramacion.com.ar/wp-content/uploads/2016/09/tap2016.pdf</a><span style="font-weight: bold;"> ]</span></p>
<div>Two years ago we had a setback when Joaqu¨ªn, a member of the jury, had an accident which prevented us from including the problem "Playing with lists" in that year's problemset for the Argentinian Programming Tournament. Thanks to the contest's participants, who kindly helped us solve that problem, we planned to include it in today's problemset. Unfortunately, we had a new inconvenience with Jacinto, another jury member.</div>
<div>&nbsp;</div>
<div>As it happens, Jacinto doesn't like it when the sample test cases included along with the problem statements span more than one page. For the problem "Playing with lists", each test case consists of a single line with the description of a list. We don't want to say too much about them because the problem is definitely going to be used next year, so for now we'll just provide you with the total number of characters for each test case, clarifying that it's not allowed to "split" a test case in order to write it in multiple lines.</div>
<div>&nbsp;</div>
<div>We would like to write the input for the <strong>N</strong>&nbsp;sample test cases in a single page, in which we can fit at most <strong>L</strong>&nbsp;lines of <strong>C</strong> characters each. The inconvenience appears when there are more sample test cases than there are lines available in the page, so that we cannot write each of them in a separate line. In order to circumvent this problem, Jacinto suggested drawing vertical segments spanning the whole height of the page, dividing it in two or more columns. These segments should have negligible width, so that the number of characters we can write in each line is not reduced, and will act as visual separators splitting each of the lines they cross. In this way, we can write each sample test case in a different line belonging to some column, as long as it doesn't cross the vertical segments. For the purposes of this problem, the order of the sample test cases is considered to be irrelevant.</div>
<div>&nbsp;</div>
<div>For example, let's consider the situation in which there are <strong>N = 5</strong>&nbsp;sample test cases in a page fitting <strong>L = 3</strong>&nbsp;lines of <strong>C = 11</strong>&nbsp;characters each. If the test cases have <strong>K<sub>1</sub>= 3</strong>, <strong>K<sub>2</sub> = 4</strong>, <strong>K<sub>3</sub> = 5</strong>, <strong>K<sub>4</sub> = 6</strong>&nbsp;and <strong>K<sub>5</sub> = 7</strong>&nbsp;characters, we can split the page in two columns in such a way that one column has a width of <strong>7</strong>&nbsp;characters, while the other one has a width of <strong>4</strong> characters. In the larger column we may write the test cases with <strong>K<sub>3</sub> = 5</strong>, <strong>K<sub>4</sub> = 6</strong>&nbsp;and <strong>K<sub>5</sub> = 7</strong>&nbsp;characters in any order, whereas in the other column we can write the remaining sample test cases, having <strong>K<sub>1</sub> = 3</strong>&nbsp;and <strong>K<sub>2</sub> = 4</strong>&nbsp;characters, again in any order.</div>
<div>&nbsp;</div>
<div>Thus, two possible ways in which we can fit the sample test cases in this example are</div>
<div>&nbsp;</div>
<div style="text-align: center;"><img title="TAP2016J.png" src="../../content/fidels:TAP2016J.png" alt="TAP2016J.png"></div>
<div style="text-align: center;">&nbsp;</div>
<div>where for example<strong> 5/7 </strong>means we have used <strong>5</strong> of the <strong>7</strong> available characters in the corresponding column.</div>
<div>&nbsp;</div>
<div>In an analogous situation for which the number of characters fitting in a single line is <strong>C = 10</strong>, we would need a column of at least <strong>7</strong>&nbsp;characters of width in order to write in it the larger sample test case. Therefore, it would be impossible to have any other column of width greater than <strong>3</strong>&nbsp;characters, which in turn means that <strong>4</strong>&nbsp;of the <strong>N = 5</strong>&nbsp;sample test cases should be written in the largest column. But this is clearly impossible, as there are only <strong>L = 3</strong>&nbsp;lines in the page. On the other hand, let us also note that although the sample test cases with <strong>K<sub>1</sub> = 3</strong>&nbsp;and <strong>K<sub>5</sub> = 7</strong>&nbsp;characters can in principle be written in a single line, as well as the sample tests cases with <strong>K<sub>2</sub> = 4</strong>&nbsp;and <strong>K<sub>4</sub> = 6</strong>&nbsp;characters, it is impossible to simultaneously put both pairs in one page in this way, as the width of each column should be the same along all the lines in the page.</div>
<div>&nbsp;</div>
<div>Now we would like your help in order to determine if it is possible to make Jacinto happy by putting all the sample test cases in a single page as described above.</div>
<p>&nbsp;</p>
<h3>Input</h3>
<p>There are multiple test cases in the input file. For each test case, the first line contains three integer numbers <strong>N</strong>, <strong>L</strong>&nbsp;and <strong>C</strong>. The integer <strong>N</strong>&nbsp;represents the number of sample test cases, <strong>L</strong>&nbsp;represents the maximum number of lines fitting in a page, and <strong>C</strong>&nbsp;represents the maximum number of characters fitting in a line (<strong>1 ¡Ü&nbsp;N, L, C <strong>¡Ü</strong>&nbsp;5000</strong>). The second line contains <strong>N</strong>&nbsp;integer numbers <strong>K<sub>1</sub></strong>, <strong>K<sub>2</sub></strong>, ..., <strong>K<sub>N</sub></strong>, representing the total number of characters in each sample test case (<strong>1 <strong>¡Ü</strong>&nbsp;K<sub>i</sub>&nbsp;<strong>¡Ü</strong>&nbsp;C</strong>&nbsp;for <strong>i = 1, 2, ..., N</strong>).</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, print a single line containing a character representing if it is possible to write all sample test cases in a single page as described in the problem statement. The printed character should be an <strong>'<span style="font-family: &quot;courier new&quot;, courier;">S</span>'</strong> if this is possible, and an <strong>'<span style="font-family: &quot;courier new&quot;, courier;">N</span>'</strong> otherwise.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: &quot;courier new&quot;, courier;">5 3 11
3 4 5 6 7
5 3 10
3 4 5 6 7
3 3 4
1 3 2
6 3 4
1 3 1 2 1 1</span>

<strong>Output:</strong>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 17.3333px; width: 1px; height: 1px; overflow: hidden;">S</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 17.3333px; width: 1px; height: 1px; overflow: hidden;">N</div><div id="_mcePaste" style="position: absolute; left: -10000px; top: 17.3333px; width: 1px; height: 1px; overflow: hidden;">S</div><span style="font-family: &quot;courier new&quot;, courier;">S
</span><div id="_mcePaste" style="position: absolute; left: -10000px; top: 17.3333px; width: 1px; height: 1px; overflow: hidden;"><span style="font-family: &quot;courier new&quot;, courier;">SS</span></div><span style="font-family: &quot;courier new&quot;, courier;">N
S
S</span></pre>