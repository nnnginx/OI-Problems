<h4>Given a large polygon dining table (not always a simple polygon) with the following properties :</h4>
<p>- there is no intersecting area (ex : area A)<br>- there is no space inside the polygon (ex : area B)<br>- there is no 3 edges that are concurrent (ex : point C)<br>- every nodes are not lying on any edge except 2 edges that connect that node with 2 other nodes (ex : point D)<br>- every nodes forming a convex corner because a table with concave corner is an uncomfortable table (ex : point E)</p>
<h4>Example of invalid table :</h4>
<p>https://drive.google.com/file/d/1_vtLBvmbej72PT1lfppdAaOIaZWR-6lg/view<br><br></p>
<h4>Given also M dishes with the following rules :</h4>
<p>- placed on the table<br>- not on the edge of the table<br>- there is no pair of different food that have the same place<br><br></p>
<h4>You have to answer Q queries :</h4>
<p>- each query identified by L and R<br>- the query is "what is the minimum moves in order to make some dishes (from L-th dish to R-th dish inclusive) placed in same region ?"<br>- queries are independent<br><br></p>
<h4>Notes :</h4>
<p>- two dishes are considered in same region if and only if from one dish can be slided to another one without crossing any edge<br>- one move is to slide a dish to another region through an edge<br>- every dishes should be still on the table, but they may lie on the edge<br><br></p>
<h4>Explanation :</h4>
<p>https://drive.google.com/file/d/1sIaODaxRhnO5biDS5jqrWAgpVI-2Q7V4/view<br>- dish A is valid because it placed on the table<br>- dish C is invalid because it placed on the edge<br>- dish E is invalid because it placed outside the table<br>- sliding from dish A to dish B is considered as one move<br>- dish B and dish D is considered as one region<br>- dish F is invalid because it placed exactly on dish D<br><br></p>
<h4>Input and output format :</h4>
<p>- An integer T represent the number of test case, each test case :<br>- First line contains 3 separated integer N, M, and Q<br>- Next N lines contain Xi and Yi represent the coordinat of i-th node<br>- Next M lines contain Pi and Qi represent the coordinat of i-th dish<br>- Next Q lines contain Li and Ri represent the parameter of i-th query<br>- You should output Q lines contain the answers of those queries<br><br></p>
<h4>Constrain :</h4>
<p>- 1 &lt;= T &lt;= 10<br>- 3 &lt;= N &lt;= 1000<br>- 2 &lt;= M &lt;= 1000<br>- 1 &lt;= Q &lt;= 1000<br>- 0 &lt;= Xi, Yi &lt;= 10^9<br>- 0 &lt; Pi, Qi &lt; 10^9<br>- 1 &lt;= Li &lt; Ri &lt;= M<br><br></p>
<h4>Sample input :</h4>
<pre>1<br>7 5 3<br>1 1<br>1 5<br>5 1<br>7 2<br>7 8<br>9 5<br>5 5<br>6 2<br>2 3<br>5 4<br>8 6<br>5 3<br>1 5<br>2 4<br>3 5</pre>
<h4>Sample output :</h4>
<pre>2<br>2<br>1</pre>
<p>&nbsp;</p>
<h4>Explanation of sample :</h4>
<p>https://drive.google.com/file/d/1OWfXYmZPo9YTrV47eh26gNhl4NMBsTY0/view</p>
<p>- query 1 : we can slide 2-nd dish and 4-th dish to the middle region<br>- query 2 : using the same way as query 1<br>- query 3 : prefer sliding 4-th dish (1 move) rather than sliding 3-rd and 5-th dishes (2 moves)</p>