<p>In Kutus and Putus¡¯ first marriage anniversary, they planned to invite all of their cat friends. So they invited all cats in a hall room. Due to business, all of the cats couldn¡¯t attend the party at the same time. Different cats attended party at different times and some of them couldn¡¯t stay till the end. Kutus wanted to make Putus as much happy as possible. If at any moment, there were ¡®L¡¯ cats present in the hall room, then happiness level of Putus were ¡®L¡¯ at that moment. Now Kutus gave you a list of every cats¡¯ arrival and departure time at the party and asked you few queries: Maximum time segment where the happiness level of Putus was ¡®L¡¯.</p>
<h3>Input</h3>
<p>Input starts with an integer <strong>T</strong>, which denotes the number of test cases. Each case contains&nbsp;<strong>2</strong>&nbsp;space separated integer&nbsp;<strong>N</strong>&nbsp;and&nbsp;<strong>Q</strong>&nbsp;denoting the number of cats came to the party&nbsp;and the number of queries to be performed. Next line contains&nbsp;<strong>N</strong>&nbsp;space separated integers ¡®<strong>X¡¯</strong> and ¡®<strong>Y</strong>¡¯ denoting the arrival time and departure time of <strong>i<sub>th</sub><sup> </sup></strong>cat. Each of the next&nbsp;<strong>Q</strong>&nbsp;lines contains an integer ¡®<strong>L</strong>¡¯ as described above.</p>
<h3>Output</h3>
<p>For each case print the case number and print the time segment ¡®<strong>X¡¯</strong> &amp; ¡®<strong>Y¡¯ </strong>that is Putus¡¯ level of happiness. If there are multiple solution, print the time segment that comes earliest. If there is no possible answer, print -1.</p>
<p><strong>Constraints:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong></p>
<p><strong>T &lt;= 10</strong></p>
<p><strong>1 &lt;= N &lt;= 100000</strong></p>
<p><strong>1 &lt;= Q &lt;= 100000</strong></p>
<p><strong>1<sup> </sup>&lt;= X<sub>i&nbsp; </sub>&lt;= Y<sub>i</sub> &lt;= 100000</strong></p>
<p><strong>1 &lt;= L &lt;= 100000&nbsp;</strong></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p>1</p><p>5 5</p><p>1 2</p><p>2 3</p><p>1 3</p><p>2 4</p><p>3 5</p><p>1</p><p>2</p><p>3</p><p>4</p><p>5</p>
<strong>Output:</strong>
<p>Case 1:</p><p>4 4</p><p>1 1</p><p>2 2</p><p>-1</p><p>-1</p></pre>