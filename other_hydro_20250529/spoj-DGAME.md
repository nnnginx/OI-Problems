<p>Digo is planning to recruit members for his ACM team, he designs a game in which who ever beats him will be recruited in his team. Darshil is a friend of yours. You have to help him get recruited in Digo's ACM team.</p>
<p>There are <strong>N</strong> piles , where <strong>i<sup>th</sup></strong> pile contains either <strong>2*i</strong> or <strong>2*i+1</strong> stones. During the game, Darshil and Digo take turns and Darshil takes the first turn. In each turn they can select any pile containing 2 or more stones and then remove an <strong>EVEN</strong> number of stones from the selected pile. The player who can't make the next move loses the game.</p>
<p>You have to find:-</p>
<p>1. Number of ways in which stones can be put in those <strong>N</strong> piles. (Each way is distinct if any one pile has different number of stones). If number of ways is <strong>M</strong> then print <strong>M</strong> % 1000000007.</p>
<p>2. For each configuration of part-1 Darshil counted the number of ways he can choose the first move such that no matter how optimally Digo plays he wins. Find the integral part of average number of such ways of all the configurations.</p>
<p><strong>Input Format</strong></p>
<p>The first line contains an integer <strong>T</strong> (number of test cases).</p>
<p>Each of the next <strong>T</strong> lines contains a single positive integer <strong>N</strong>.</p>
<p><strong>Output Format</strong></p>
<p><strong>T</strong> lines containing two space-separated integers - the answers to the first and second parts of the questions.</p>
<p><strong>Constraints </strong></p>
<p>1 &lt;= <strong>N</strong> &lt;= 10^9</p>
<p>1 &lt;= <strong>T</strong> &lt;= 10^3</p>
<p><strong>Sample Input</strong></p>
<p>3</p>
<p>1</p>
<p>2</p>
<p>3</p>
<p><strong>Sample Output</strong></p>
<p>2 1</p>
<p>4 1</p>
<p>8 0</p>