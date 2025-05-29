<p style="text-align: center;"><strong>PROBLEM E</strong></p>
<p style="text-align: center;"><strong>&nbsp;PUBLISH OF PERISH</strong></p>
<p>“Publish or perish” is the academic life’s fundamental motto. It refers to the fact that publishing your work frequently is the only way to guarantee access to research funds, bright students and career advances. But publishing is not enough. It is necessary that your work is <em>referenced </em>(or <em>cited</em>). That is, your papers must be mentioned as source of information in other people’s publications, to attest the quality and relevance of your research. The more citations a paper receives from other authors, the more it is considered influential.</p>
<p>In 2005 Jorge E. Hirsch, a physicist at the University of California at San Diego, proposed a way to evaluate the scientific impact of a researcher, based on the citations his or her papers have received. The <em>h-index</em>, as Hirsch’s proposal became known, is a number based on the set of a researcher’s most cited papers. It is defined in Hirsch’s own words as: A scientist has index h if h of his N<sub>p</sub> papers have at least h citations each, and the other (N<sub>p</sub> − h) papers have at most h citations each.</p>
<p>Albert Einstein, for example, published 319 papers in scientific journals and has an h-index equal to 46. It means 46 of his papers have received 46 or more citations each, and all of his remaining 273 papers have 46 citations or less each. Given the information of how many citations each paper from a given researcher has received, write a program to calculate that researcher’s h-index.</p>
<p><strong>Input</strong></p>
<p>The input contains several test cases. The first line of a test case contains one integer N indicating the number of papers a researcher has published (1&lt;=N&lt;=10<sup>3</sup>). The second line contains a list of N integers M<sub>i</sub>, separated by one space, representing the number of citations each of the N papers from that author has received (0&lt;=M<sub>i</sub> &lt;=10<sup>3</sup>, for 1&lt;= i &lt;= N). The end of input is indicated by a line containing only one zero.<strong></strong></p>
<p><strong>Output</strong></p>
<p>For each test case in the input, your program must print a single line, containing one single integer, the h-index for the given list of citations.<strong></strong></p>
<p><strong>Sample Input</strong></p>
<p>4</p>
<p>1003 1 200 2</p>
<p>10</p>
<p>1 1 1 0 1 1 0 1 1 1</p>
<p>7</p>
<p>6 5 4 3 2 1 0</p>
<p>0</p>
<p><strong>Sample Output</strong></p>
<p>2</p>
<p>1</p>
<p>3</p>