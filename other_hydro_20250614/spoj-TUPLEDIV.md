<p><strong>Description</strong></p>
<p>You are given N tuples with M dimensions. You need to choose some tuples and divide them into M groups. Each tuple can be used for only once and the size of the i<sup>th</sup> group is C<sub>i</sub>. We define the score of the i<sup>th</sup> group is the sum of value in the i<sup>th</sup> dimension of the tuples in the i<sup>th</sup> group. Your target is to firstly maximize the score of 1<sup>th</sup> group, then maximize the score 2<sup>th</sup> group and so on.&nbsp;</p>
<p><strong>Input</strong></p>
<p>The first line of the input contains an integer T(T¡Ü50), indicating the number of cases. Each case begins with two integer N(1¡ÜN¡Ü10000) and M(1¡ÜM¡Ü10), the number of tuples and the number of groups. Then there is one line contain M integers. The i<sup>th</sup> integer C<sub>i </sub>(C<sub>i</sub> &gt;=0, sigma C<sub>i</sub> &lt;= N) represents the size of the i<sup>th</sup> group. Then N lines with M integers follow. Each of them describes a tuple. The j<sup>th</sup> integer on the i<sup>th</sup> line T<sub>ij</sub> (0 &lt;=T<sub>ij</sub> &lt;= 10000) denotes the value of the j<sup>th</sup> dimension of the i<sup>th</sup> tuple.</p>
<p><strong>Output</strong></p>
<p>For each test case, print one line with M score of some optimal division.</p>
<p><strong>Sample Input</strong></p>
<p>2</p>
<p>4 2</p>
<p>2 1</p>
<p>3 2</p>
<p>2 1</p>
<p>2 2</p>
<p>1 1</p>
<p>4 3</p>
<p>1 1 2</p>
<p>8 7 1</p>
<p>8 7 2</p>
<p>8 7 4</p>
<p>8 2 3</p>
<p><strong>Sample Output</strong></p>
<p>5 2</p>
<p>8 7 7</p>
<p><strong>Hint</strong></p>
<p>In case 2, we can dive the group like:</p>
<p>Group 1: (8, 7, 2)&nbsp; score = 8</p>
<p>Group 2: (8, 7, 1)&nbsp; score = 7</p>
<p>Group 3: (8, 7, 4), (8, 2, 3) score = 4 + 3 = 7</p>
<p>&nbsp;</p>