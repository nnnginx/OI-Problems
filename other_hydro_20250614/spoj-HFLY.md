<pre style="text-align: justify;"><br><span style="white-space: normal;"><h3 style="color: #333333; text-align: center;"><span style="font-size: xx-large;">Airplane Parking</span></h3><p style="font-family: 'Times New Roman'; font-size: medium;">During this economic crisis time, Jack has started an incredible new business related to air travel, a parking-lot for airplane. He bought a very large land to park airplanes. However the land is very narrow, so that the only way airplanes can go in or go out of the parking lot must be in the&nbsp;Last-In First-Out&nbsp;fashion (see picture below). He only has spaces in the parking lot so he&nbsp;cannot&nbsp;take some airplane at the end out so that other airplanes can move.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<div style="font-family: 'Times New Roman'; font-size: medium;"><img src="../../../../../../content/simes:HFLY.jpg" border="0" align="BOTTOM"></div>
<p style="font-family: 'Times New Roman'; font-size: medium;">Because of the limitation of the parking lot, it is not possible to accommodate all requests for parking. Each request consists of the planned arrival time and planned departure time, which are the times the airplane arrives at the parking lot. An example below shows a request table for 4 planes.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<div style="font-family: 'Times New Roman'; font-size: medium;">
<table border="0" frame="BOX" rules="GROUPS">
<colgroup><col align="CENTER"></colgroup><colgroup><col align="CENTER"></colgroup><colgroup><col align="CENTER"></colgroup>
<tbody>
<tr>
<td align="CENTER" valign="BASELINE">Airplane</td>
<td align="CENTER" valign="BASELINE">Arrival</td>
<td align="CENTER" valign="BASELINE">Departure</td>
</tr>
</tbody>
<tbody>
<tr>
<td align="CENTER" valign="BASELINE">1</td>
<td align="CENTER" valign="BASELINE">1</td>
<td align="CENTER" valign="BASELINE">10</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">2</td>
<td align="CENTER" valign="BASELINE">2</td>
<td align="CENTER" valign="BASELINE">5</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">3</td>
<td align="CENTER" valign="BASELINE">3</td>
<td align="CENTER" valign="BASELINE">7</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">4</td>
<td align="CENTER" valign="BASELINE">6</td>
<td align="CENTER" valign="BASELINE">9</td>
</tr>
</tbody>
</table>
</div>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<p style="font-family: 'Times New Roman'; font-size: medium;"><br>In this case, it is possible to accommodate airplane 1, 2, and 4. But it is not possible to accommodate both airplanes 2 and 3.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">It is possible that different planes plan to arrive or depart the parking lot at the same time. Jack has the best crews working with him, so that they will manage to arrange the plane to the parking lot in the best way that if it is possible to park and take out the planes they will be able to do it. Consider another example.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<div style="font-family: 'Times New Roman'; font-size: medium;">
<table border="0" frame="BOX" rules="GROUPS">
<colgroup><col align="CENTER"></colgroup><colgroup><col align="CENTER"></colgroup><colgroup><col align="CENTER"></colgroup>
<tbody>
<tr>
<td align="CENTER" valign="BASELINE">Airplane</td>
<td align="CENTER" valign="BASELINE">Arrival</td>
<td align="CENTER" valign="BASELINE">Departure</td>
</tr>
</tbody>
<tbody>
<tr>
<td align="CENTER" valign="BASELINE">5</td>
<td align="CENTER" valign="BASELINE">10</td>
<td align="CENTER" valign="BASELINE">12</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">6</td>
<td align="CENTER" valign="BASELINE">10</td>
<td align="CENTER" valign="BASELINE">15</td>
</tr>
<tr>
<td align="CENTER" valign="BASELINE">7</td>
<td align="CENTER" valign="BASELINE">13</td>
<td align="CENTER" valign="BASELINE">17</td>
</tr>
</tbody>
</table>
</div>
<p style="font-family: 'Times New Roman'; font-size: medium;">&nbsp;</p>
<p style="font-family: 'Times New Roman'; font-size: medium;"><br>Although airplane 5 and 6 arrive at the same time, Jack's crews know that airplane 5 will have to be out before airplane 6, so when both airplanes arrive they put airplane 6 in first, following by airplane 5.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">Given a list of parking requests, you want to find the maximum number of airplanes that can be parked in this parking lot, provided that they can only depart in the Last-In First-Out fashion.</p>
<h2><span style="font-size: x-large;">Input</span></h2>
<p style="font-family: 'Times New Roman'; font-size: medium;">The first line contains an integer&nbsp;<em>T</em>, the number of test cases&nbsp;(1<img src="file://hgCCpbMb.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>T</em><img src="file://U2IJcmWp.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">5). Each test case is in the following format.</p>
<p style="font-family: 'Times New Roman'; font-size: medium;">The first line starts with an integer&nbsp;<em>N</em>&nbsp;(1<img src="file://pomnfrts.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>N</em><img src="file://1kOcjrdw.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">300)&nbsp;denoting the number of airplanes. The next&nbsp;<em>N</em>&nbsp;lines describe the request table. Each line&nbsp;1 +&nbsp;<em>i</em>, for&nbsp;1<img src="file://xolAFYLp.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>i</em><img src="file://zlTb9gn4.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>N</em>, contains two integer&nbsp;<em>S</em><sub>i</sub>&nbsp;and&nbsp;<em>T</em><sub>i</sub>&nbsp;,&nbsp;(0<img src="file://Sxj2EWuJ.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE"><em>S</em><sub>i</sub>&nbsp;&lt;&nbsp;<em>T</em><sub>i</sub><img src="file://JJZePN1f.png" border="0" alt="$ \le$" width="18" height="31" align="MIDDLE">1, 000, 000, 000)&nbsp;which are the planned arrival time and planned departing time for airplane&nbsp;<em>i</em>.</p>
<p><span style="font-size: x-large;"><strong>Output</strong></span></p>
<p>&nbsp;</p>
<p>For each test case, you program must output a single line consisting of one integer, the maximum number of airplanes that can be parked in Jack's parking lot.</p>
<p>&nbsp;</p>
<p><span style="font-size: x-large;"><strong>Sample Input</strong></span></p>
<p>2</p>
<p>4</p>
<p>1 10</p>
<p>2 5</p>
<p>3 7</p>
<p>6 9</p>
<p>3</p>
<p>10 12</p>
<p>10 15</p>
<p>13 17</p>
<p><span style="font-size: x-large;"><strong>Sample Output</strong></span></p>
<p>3</p>
<p style="text-align: justify;">2</p>
</span></pre>