<div>
<div id="problem-statement-preview">
<p>Alia  is world¡¯s most widely acclaimed cryptographer. Recently she developed a  new way to encrypt passwords over the internet. Instead of using the  secret ¡°Key¡±, now she intends to use a secret ¡°Key Matrix¡± for  encryption.</p>
<p>The ¡°Key Matrix¡± consists of an integer matrix of dimensions m * n.  Besides, there are four coordinates x1, y1, x2, y2. The ¡°Key¡± can be  retrieved from ¡°Key Matrix¡± performing bitwise XOR(^) operation over all  the integers present in rectangle having its upper left corner as (x1,  y1) and lower right index as (x2, y2). (Note:  the matrix is 0 based)  Also Alia has developed new tools to regularly update his key to protect  it from ¡°attackers¡±. So she will update the values of some cells from  time to time. You friend, being an expert hacker has finally retrieve  the ¡°Key Matrix¡± . Now he only needs to use the matrix to retrieve the  key. Since this appears to be a tedious task, he turns to you. Help your  friend by retrieving the secret ¡°key¡± from the ¡°key matrix¡±.</p>
<p>In brief, you¡¯ll have to do the following two operations over the matrix</p>
<p>0 x1 y1 x2 y2 : Perform the XOR of all the integers present in the  rectangle having its upper left corner as (x1, y1) and lower right index  as (x2, y2).</p>
<p>1 x1 y1 k:  Update the value at position (x1, y1) by k.</p>
<p><strong>Input:</strong></p>
<p>The first line of input will contain integers m and n (separated with space) specifying the dimensions of the  matrix. This is followed by a m * n matrix (m rows and n columns) denoting the ¡°Key Matrix¡±. The next line contains an integer q denoting the number of queries. Each of the following q lines contains a single query in the specified  format.</p>
<p><strong>Output:</strong></p>
<p>For each query, print the value of the secret ¡°Key¡± that you retrieve from the ¡°Key Matrix¡±</p>
<p><strong>Constraints</strong></p>
<p>1 &lt;= m, n &lt; 600</p>
<p>1 &lt;= q &lt;= 20,000</p>
<p>0 &lt;= x1, x2 &lt;= m ¨C 1</p>
<p>0 &lt;= y1, y2 &lt;= n ¨C 1</p>
<p>0 &lt;= Aij, k &lt;= 10^8</p>
<p><strong>Sample Input:</strong></p>
<p>2 2</p>
<p>1 2</p>
<p>3 4</p>
<p>2</p>
<p>1 0 0 2</p>
<p>0 0 0 1 1</p>
<p><strong>Sample Ouptut:</strong></p>
<p>7</p>
<p><strong>Explanation</strong></p>
<p>The first query updates the value of (0, 0) to 2. Now the Key matrix appears like 2 2 3 4 Now for query 2 the secret key is the XOR of the value in the entire matrix So the key is 2 ^ 2 ^ 3 ^ 4 = 7</p>
</div>
</div>