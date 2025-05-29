<p>After Mr. B arrived in Warsaw, he was shocked by the skyscrapers and took several photos. But now when he looks at these photos, he finds in surprise that he isn't even able to point out the number of buildings in it. So he decides to work it out as follows:</p>
<p>- divide the photo into n vertical pieces from left to right. The buildings in the photo can be treated as rectangles, the lower edge of which is the horizon. One building may span several consecutive pieces, but each piece can only contain one visible building, or no buildings at all.</p>
<p>- measure the height of each building in that piece.</p>
<p>- write a program to calculate the minimum number of buildings.</p>
<p>Mr. B has finished the first two steps, the remaining comes to you.</p>
<h3>Input</h3>
<p>Each test case starts with a line containing an integer <strong>n</strong> (1 &lt;= <strong>n</strong> &lt;= 100,000). Following this is a line containing <strong>n</strong> integers - the height of building in each piece respectively. Note that zero height means there are no buildings in this piece at all. All the input numbers will be nonnegative and less than 1,000,000,000.</p>
<h3>Output</h3>
<p>For each test case, display a single line containing the case number and the minimum possible number of buildings in the photo.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1 2 3
3
1 2 1

<strong>Output:</strong>
Case 1: 3
Case 2: 2
</pre>
<p><strong>Explanation</strong></p>
<p>The possible configurations of the samples are illustrated below:</p>
<p><img src="../../../content/john_jones:city2.jpg" alt=""></p>