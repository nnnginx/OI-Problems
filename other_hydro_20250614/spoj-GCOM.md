<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Binary Representation of a number represents a point (vertex) in the N-th dimensional hyper-cube (N is the number of bits used to represent the number in binary form ) . Eg. point 3(011) and 5(101) are shown in 3-dimensional figure. As the value of points increases, number of axes to represent it in the hyper-cube increases .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Given an N-th dimensional hyper-cube and an array (of size n ) of selected points from the cube&nbsp; . We select its complementary point from the cube . We call communication between these points " GOOD " if the distance between given point and its complementary point is maximum . Distance between two points is defined as the bitwise XOR of two points . Let this complementary point be M . The cost of building communication between them is given by</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;Cost = 2 ^ (n) ; where n is position of unset bit which is at farthest distance from MSB in M</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">To decrease the cost we have two operations :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Type1: ' q l r ' :- it returns the point which has minimum cost of building the communication . In case there are multiple answers , print the point with minimun value&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Type2: ' u x y ' :- update the point at index x with value y&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">NOTE:- ' l r x ' are according to 1-based indexing&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 20</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= n , q &lt;= 105</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= array elements &lt;= 109</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input:&nbsp; First Line contains number of test cases. Next Line contains n and q representing size of array and number of operations . Next line contains array elements . Next q lines operations of type1 and type2 in the specified format&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output: Give answer of the required type in new lines .</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Example</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2 3 4&nbsp; &nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">q 1 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">u 2 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">q 1 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">&nbsp;</div>
<p><img style="vertical-align: middle;" src="./22560/file/NoEgFq7E.png" alt="" width="500" height="395"></p>
<p>Image Link : In case image is not visible ( <a href="https://drive.google.com/file/d/1w81eNDnNnwQCbPsBJyHoMICVpN7-ml-Y/view?usp=sharing" target="_blank">Link</a> )</p>
<p>&nbsp;</p>
<p>Binary Representation of a number represents a point (vertex) in the N-th dimensional hyper-cube (N is the number of bits used to represent the number in binary form ) . Eg. point 3(011) and 5(101) are shown in 3-dimensional cube in the figure. As the value of points increases, number of axes to represent it in the hyper-cube increases .</p>
<p>&nbsp;</p>
<p>Given an N-th dimensional hyper-cube and an array (of size n ) of selected points from the cube&nbsp; . We select its complementary point from the cube . We call communication between these points " GOOD " if the distance between given point and its complementary point is maximum . Distance between two points is defined as the bitwise XOR of two points . Let this complementary point be M . The cost of building communication between them is given by</p>
<p>&nbsp;</p>
<p>&nbsp;Cost = 2 <sup>(n)</sup> ; where n is position of unset bit which is at farthest distance from MSB in M</p>
<p>&nbsp;</p>
<p>To decrease the cost we have two operations :</p>
<p>&nbsp;</p>
<p>Type1: ' q l r ' :- we select two positions l and r from the array. Output the point from the array, between the smaller and larger position being selected , which has minimum cost of building the communication .In case there are multiple answers , print the point with minimun value&nbsp;</p>
<p>&nbsp;</p>
<p>Type2: ' u x y ' :- update the point at index x with value y&nbsp;</p>
<p>&nbsp;</p>
<p>NOTE:- ' l r x ' are according to 1-based indexing (1 &lt;= l,r &lt;= n)&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong></p>
<p>&nbsp;</p>
<p>1 &lt;= T &lt;= 20</p>
<p>&nbsp;</p>
<p>1 &lt;= n , q &lt;= 10<sup>5</sup></p>
<p>&nbsp;</p>
<p>1 &lt;= array elements &lt;= 10<sup>9</sup></p>
<p>&nbsp;</p>
<p><strong>Input:</strong>&nbsp; First Line contains number of test cases. Next Line contains n and q representing size of array and number of operations . Next line contains array elements . Next q lines operations of type1 and type2 in the specified format&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Output:</strong> Give answer of the required type in new lines .</p>
<p>&nbsp;</p>
<hr>
<p>&nbsp;</p>
<p><strong>Example</strong></p>
<p>&nbsp;</p>
<p>Input</p>
<p>&nbsp;</p>
<p>1</p>
<p>&nbsp;</p>
<p>3 3</p>
<p>&nbsp;</p>
<p>2 3 4&nbsp; &nbsp;</p>
<p>&nbsp;</p>
<p>q 1 3</p>
<p>&nbsp;</p>
<p>u 2 5</p>
<p>&nbsp;</p>
<p>q 1 2</p>
<p>&nbsp;</p>
<p>Output</p>
<p>&nbsp;</p>
<p>3</p>
<p>&nbsp;</p>
<p>5</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>