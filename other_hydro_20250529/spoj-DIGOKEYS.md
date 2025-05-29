<p>A psychic lock-lover called Digo likes playing games with Locks and Keys and also has very good logic.</p>
<p>One day he buys a set of <strong>N</strong> boxes, each of them has an index between {<strong>1, N</strong>} (inclusive) and no two boxes have same index. There is a key inside every box except the <strong>Nth</strong> box which has great treasure. He eventually finds out that due to a defect in the manufacturing of the keys, most of them could open more than one box.</p>
<p>The rule is that you are allowed to open only one box with any key. Each box except the first is locked. Now as Digo couldn¡¯t wait long to acquire that great treasure he requests you to find a method to open the last box starting with the key in the first box with minimum number of steps.</p>
<p><strong>INPUT</strong></p>
<p>In first line, <strong>T</strong> no. of test cases.</p>
<p>For every test case:</p>
<p>In first line, there is an integer <strong>N</strong> : (number of locks)</p>
<p>In next <strong>N-1</strong> lines, on the <strong>i¡¯th</strong> line there is an integer <strong>Mi </strong>the number of boxes which the key present in the <strong>i¡¯th </strong>box<strong> </strong>can open. It is followed by the <strong>Mi</strong> integers (the indices of those boxes that can be opened by the key present in <strong>i¡¯th</strong> box).</p>
<p><strong>OUTPUT</strong></p>
<p>For every test case:</p>
<p>one integer <strong>q</strong>, minimum number of boxes opened.</p>
<p>In the next line : &nbsp;the indices of the boxes opened in order separated by space. If there are many solutions print the one which is lexicographically smallest.</p>
<p>If there is no way to reach the last box print ¡°-1¡±.</p>
<p>Each test case is to be followed by a blank line.<strong> </strong></p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= <strong>T</strong> &lt;= 10</p>
<p>2 &lt;= <strong>N</strong> &lt;= 100000</p>
<p>1 &lt;= <strong>Mi</strong> &lt;= 10<strong></strong></p>
<p><strong>Sample Input</strong></p>
<p>2</p>
<p>3</p>
<p>1 2</p>
<p>1 3</p>
<p>4</p>
<p>2 2 3</p>
<p>1 1</p>
<p>2 2 4</p>
<p><strong>Sample Output</strong></p>
<p>2</p>
<p>1 2</p>
<p>&nbsp;</p>
<p>2</p>
<p>1 3</p>