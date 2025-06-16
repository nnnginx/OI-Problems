<p><span style="font-size: small;">On day 1, a mobile manufacturing company bought L quantities of raw materials which can produce exactly L mobile phones. The raw materials are then transported to factories.</span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">The company owns M factories located at various locations where these raw materials are converted into mobile phones. ith factory is capable of producing atmost F[i] mobile phones provided the availability of raw materials.</span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">The manufactured mobile phones can be transported to N shops at various locations where these mobile phones are sold. Each shop has a selling capability. ith shop can sell atmost S[i] mobile phones in a day. You are given a 2D map of order MxN. ith factory can transport atmost map[i][j] mobile phones to jth shop.</span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><span style="font-size: small;">Find the maximum number of mobile phones that can be sold by the company on day 1. For simplicity you can assume that the time taken for transportation of raw materials and mobiles as 0.</span></span></span></p>
<p><span style="font-size: small;"><br></span></p>
<p><span style="font-size: small;"><strong><span style="font-size: small;"><br>Input:</span></strong></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">The first line consists of an integer t, the number of test cases. For each test case, the first line consists of 3 integers L, M and N. The next line consists of M integers representing the array F. The next line consists of N integers representing the array S. The next M lines represent the map.</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-family: tahoma, arial, helvetica, sans-serif;"><span style="font-size: small;"><strong><span style="font-size: small;">Output:</span></strong></span></span></p>
<p><span style="font-family: tahoma, arial, helvetica, sans-serif;"><span style="font-size: small;"><span style="font-size: small;">For each test case, find the maximum number of mobile phones that can be sold by the company on day 1.</span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-family: tahoma, arial, helvetica, sans-serif;"><span style="font-size: small;"><strong><span style="font-size: small;">Input Constraints:</span></strong></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= t &lt;= 100</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= L &lt;= 1000</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= M &lt;= 200</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">1 &lt;= N &lt;= 200</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">0 &lt;= F[i] &lt;= 1000</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">0 &lt;= S[i] &lt;= 1000</span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">0 &lt;= map[i][j] <span style="color: #545454;"><span style="line-height: 14.5600004196167px;">&lt;= 1000</span></span></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;"><br></span></span></p>
<p><span style="font-family: tahoma, arial, helvetica, sans-serif;"><span style="font-size: small;"><strong><span style="font-size: small;">Sample Input:</span></strong></span></span></p>
<p><span style="font-size: x-small;"><span style="font-size: small;">2<br></span></span><span style="font-size: small;">5 2 2<br></span><span style="font-size: small;">3 5<br></span><span style="font-size: small;">2 3<br></span><span style="font-size: small;">1 2<br></span><span style="font-size: small;">1 0<br></span><span style="font-size: small;">3 3 1<br></span><span style="font-size: small;">3 4 4<br></span><span style="font-size: small;">4<br></span><span style="font-size: small;">1<br></span><span style="font-size: small;">2<br></span><span style="font-size: small;">2</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">3 3 1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">3 4 4&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">4&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">1&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">2&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 570.4px; width: 1px; height: 1px; overflow: hidden;">2</div>
<p><span style="font-family: tahoma, arial, helvetica, sans-serif;"><span style="font-size: small;"><strong><span style="font-size: small;">Sample Output:</span></strong></span></span></p>
<p><span style="font-size: small;"><span style="font-size: small;">4<br></span></span><span style="font-size: small;">3</span></p>
<p><span style="font-size: small;">See Also :<strong> <a href="../../problems/SELLPHON">Mobile Company 1</a></strong></span></p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>
<p>
<script src="data:text/javascript;base64,JCgnI3Byb2JsZW0tdGFncycpLmhpZGUoKQ=="></script>
</p>