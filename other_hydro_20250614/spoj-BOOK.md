<p>Bob has a difficult job. He must distribute advertising booklets for extra school activities in different schools. The booklets have different number of pages. Bob has a list with the number of pages of each booklet and the number of schools that he must visit. He has to distribute the booklets such that each school gets a number of booklets equal to either the lower integer part (LIP),or the upper integer part (UIP) of the number of booklets divided by the number of schools. Poor Bob must obey other rules too. He must distribute all the <b>UIP</b> number of booklets first and then the <b>LIP</b> number of booklets.</p>
<p>Any booklet <b>A</b> that is distributed to a school <b>S_i</b> must have fewer or at most an equal number of pages that any other booklet B that is distributed to a school <b>S_j</b>, if <b>S_i</b> gets the booklets before <b>S_j</b> (i.e if <b>i</b> &lt; <b>j</b> then <b>pages(A)</b> &lt;= <b>pages(B)</b>). When Bob distributes the booklets to a school he must distribute them in the same relative order in which they are on his list.</p>
<p>Moreover, he must distribute them very fast. When he comes back to the advertising company his boss verifies if he accomplished well his task, by asking him the number of pages of the first booklet distributed to a specific school, following the order in which Bob visited the schools (starting with 0). Difficult job, isn't it? Can you help him?</p>

<h3>Input</h3>
<p>The input starts with a line containing a single integer <b>t</b> &lt;= 20, the number of test cases. <b>t</b> test cases follow.</p>
<p>Each data set in the input stands for a particular set of bookets. For each set of booklets the input contains the number of schools, the school specified by Bob's boss, the number of booklets (<b>less than 3000</b>), the number of pages of each booklet (fits in integer). White spaces can occur freely between the numbers in the input. The input data are correct.</p>

<h3>Output</h3>
<p>For each set of data the program prints the result to the standard output on a separate line. The solution is represented by the number of pages of the first booklet distributed to the specified school.</p>

<h3>Example</h3>

<pre><b>Input:</b>
1
3
2
7
3 5 9 1 11 14 2

<b>Output:</b>
11
</pre>