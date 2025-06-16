<p>There are <strong>N</strong> customers set their <strong>M</strong> different advertisements on Baidu. Each advertisement is owned by single customer. The ads system of Baidu records the number of clicks of each advertisement this year. The proposal system wants to analysis the advertisements about the relativity of the description length and the number of clicks of the advertisements. During the analysis, it is very important to do such a query to ask the total length of the advertisements with top <strong>K</strong> clicking times for each customer. You may assume the clicks of all advertisements are distinct.</p>
<p>Your task is to help Baidu to design this little toolkit.</p>
<h3>Input</h3>
<p>The input consist multiple test cases. The number of test cases is given in the first line of the input.</p>
<p>For each test case, the first line contains three integers <strong>N</strong>, <strong>M</strong> and <strong>Q</strong>, denoting the number customer, the number of advertisement instances and the number of queries. (<strong>N</strong> &lt;= 100000, <strong>M</strong> &lt;= 500000, <strong>Q</strong> &lt;= 100000)</p>
<p>Then <strong>M</strong> lines follow, each line contains three numbers, <strong>U</strong>, <strong>C</strong> and <strong>L</strong>, indicating the owner of this advertisement, the clicks for this advertisement and the length.</p>
<p>Finally <strong>Q</strong> lines come. Each line contains only one integer <strong>K</strong>, representing the query for top <strong>K</strong> clicking advertisements for each customer.</p>
<p>All input numbers will be positive and less than 1000000000.</p>
<h3>Output</h3>
<p>For each test case, output <strong>Q</strong> lines, each line contains only one integer, denoting the sum of total length of the top <strong>K</strong> number of clicks for each customer.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
2 4 3
1 12 13
2 23 41
1 21 46
1 22 31
1
2
3
6 15 3
5 2677139 731358928
2 347112028 239095183
6 27407970 85994789
6 767687908 734935764
6 255454855 110193353
3 39860954 813158671
5 617524049 55413590
3 338773814 7907652
6 810348880 736644178
2 777664288 63811422
6 590330120 616490361
5 552407488 136492190
1 416295130 448298060
5 811513162 232437061
4 43273262 874901209
4
9
13

<strong>Output:</strong>
Case #1:
72
118
131
Case #2:
5801137622
5887132411
5887132411
</pre>
<pre><strong>Warning: large input/output data, be careful with certain languages</strong></pre>