<p align="justify">Every non-empty sequence of elements 0 and 1 is called a binary word. A word equation is an equation of the form <i>x</i><sub>1</sub><i>x</i><sub>2</sub>...<i>x<sub>l</sub></i> = <i>y</i><sub>1</sub><i>y</i><sub>2</sub>...<i>y</i><i><sub>r</sub></i>, where <i>x</i><i><sub>i</sub></i> and <i>y</i><i><sub>j</sub></i> are binary digits (0 or 1) or variables i.e. small letters of English alphabet. For every variable there is a fixed length of the binary words that can be substituted for this variable. This length is called a length of variable. In order to solve a word equation we have to assign binary words of appropriate length to all variables (the length of the word assigned to the variable <i>x</i> has to be equal to the length of this variable) in such a way that if we substitute words for variables then both sides of the equation (which are binary words after substitution) become equal. </p>
<p align="justify">For a given equation compute how many distinct solutions it has.</p>

<h3>Example</h3>
<p align="justify">Let <tt>a</tt>, <tt>b</tt>, <tt>c</tt>, <tt>d</tt>, <tt>e</tt> be variables and let 4, 2, 4, 4, 2 be their lengths (4 is the length of <tt>a</tt>, 2 is the length of <tt>b</tt> etc.). Consider the equation:</p>
<p align="justify"><tt>1bad1 = acbe</tt></p>
<p align="justify">This equation has 16 distinct solutions.</p>

<h3>Input</h3>
<p align="justify">The number of equations <i>t</i> is in the first line of input, then <i>t</i> descriptions of equations follow separated by an empty line.</p>
<p align="justify">Each description consists of 6 lines. An equation is described in the following way: in the first line of the description there is an integer <i>k</i>, 0 &lt;= <i>k</i> &lt;= 26, which denotes the number of distinct variables in the equation. We assume that variables are the first <i>k</i> small letters of English alphabet. In the second line there is a sequence of <i>k</i> positive integers separated by single spaces. These numbers denote the lengths of variables <tt>a</tt>, <tt>b</tt>, ... from the equation (the first number is the length of <tt>a</tt>, the second - <tt>b</tt>, etc.). There is an integer <i>l</i> in the third line of the description, which is the length of the left size of equation, i.e. the length of the word built of digits 0 or 1 and variables (single letters). The left side of the equation is written in the next line as a sequence of digits and variables with no spaces between them. The next two lines contain the description of the right side of the equation. The first of these lines contains a positive integer <i>r</i>, which is the length of the right side of the equation. The second line contains the right side of the equation which is encoded in the same way as the left side. The number of digits plus sum of the lengths of variables (we count all appearances of variables) on each side of the equation is not greater than 10000. </p>

<h3>Output</h3>
<p align="justify">For each equation your program should output one line with the number of distinct solutions.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5
4 2 4 4 2
5
1bad1
4
acbe

<b><tt>Sample output:</tt></b>
16
</pre>