<p>Professor Z. has a courtyard beside his house. In the past, he loved to clean it and prune the flowers in his yard. However, with the JavaFF class taught by Professor Z. being offered, he indulged in assigning boring homework to the students and had no time for caring his yard. 

</p><p>Consequently, weeds begin to grow up and then his yard becomes overgrown. In the last weekend, after Professor Z. assigned a mass of boring homework again, he suddenly brought his yard to mind. And after he saw the weedy ground, he decided to remove the weeds. But he did not have much time to deal with the garden��s problem because of the uncompleted plans of further boring homework in the next JavaFF class.&nbsp; 

</p><p>He sprayed herbicide on the ground optionally and, strangely, herbicide was sprayed as several simple polygons on the ground. In order to determine whether he should continue his work or not, Professor Z. needed to know how many weeds were covered by the herbicide. 

</p><p>Notice that we assume that the weeds were not killed by the herbicide applied before. In the other words, a single weed can be counted several times in different polygon of herbicide. It seems that counting this number is quite a tough job. Then he asked Maryanna, one of his students in JavaFF class, for help. But Maryanna has no time because her boring homework had never been finished. Please help her! 

</p><h3>Input</h3>
<p>The very first line of input contains an integer <b>T</b> (<b>T</b> &lt;= 100) indicating the number of test cases. The first line of each test case is an integer <b>N</b> (<b>N</b> &lt;= 1000), which is the number of weeds in Professor Z's yard. In the following <b>N</b> lines, each line has a pair of integers (Xi, Yi) denoting the coordinate of a weed (-10000 &lt;= Xi, Yi &lt;= 10000). You can assume all the coordinates are unique. The next line is an integer <b>M</b> (<b>M</b> &lt;= 1000) which denotes the number of polygons covered by herbicide, all these polygon's vertices are located on one of the <b>N</b> weeds, then <b>M</b> polygons descriptions are following. Each polygon Pi has two lines, the first line of <i>i</i>th polygon has an integer Si (3 &lt;= Si &lt;= N) denoting the number of vertices in this polygon. The following line contains Si integers, describing the vertices of this polygon in clockwise or counter-clockwise order. In detail, each integer in this line is an index of the coordinates of the N weeds listed before. Notice that the indexes start from 1. See the sample input for further details. 

</p><h3>Output</h3>
<p>For each test case, output <b>M</b> lines, each line has a single integer indicating the number of weeds covered by the corresponding polygon. If a weed lies on the edge of a polygon, then we consider such a weed as being covered. 

</p><h3>Example</h3>
<pre><b>Input:</b>
1
6
1 1
3 2
2 3
1 -1
-1 -2
-1 1
3
3 5 4 3
3 1 5 6
5 5 4 2 3 6

<b>Output:</b>
Case #1:
4
3
6
</pre>