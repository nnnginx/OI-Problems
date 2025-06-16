<p>Alex has a huge farm land. Annual Farm Land Health Analysis Report by government revealed that some parts of his farms are rich in lot of valuable minerals. Now government want to conduct an air borne survey of his farm using huge laser devices attached to helicopters to calculate the exact quantity of minerals present in the farm. Each of these laser device has a rectangular base consisting of thousands of laser pores such that projection of device base on the ground will be analysed. These devices can be of different dimensions.<br><br>Now such survey will destroy the newly grown crops in the farm area that will be analysed. Government has sent Alex the map having the locations at which these devices will be used over his farms. Now Alex want to know how much crop would be left in the farm as compensation from the government for destroyed crop will take some time. Help Alex to identify the area of his farm land that will not be damaged by this survey. No device will inspect the surface outside the farm. To get more accurate mineral analysis same surface might be analysed by multiple devices. You can assume all devices will be parallel to the ground during the survey.</p>
<h3>Input</h3>
<p>First line of input contains 4 integers FX1, FY1, FX2, FY2 denoting the rectangular farm land owned by Alex.<br>Next line of input contains and integer N denoting number of laser devices that will be used. <br>Following N lines contains the location of these devices in the farm map. Every location is specified by 4 integers i.e. (x1,y1) and (x2,y2) which denotes the rectangular base of the device.</p>
<h3>Output</h3>
<p>Area of farm owned by Alex that will not be destroyed by the survey.</p>
<h3>Constraints:</h3>
<p>1 &lt;= N &lt;= 100000<br>-10^8 &lt;= fx1,fx2,fy1,fy2,x1,x2,y1,y2 &lt;= 10^8<br>min(fx1,fx2) &lt;= x1,x2 &lt;= max(fx1,fx2)<br>min(fy1,fy2) &lt;= y1,y2 &lt;= max(fy1,fy2)</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
-10 -10 10 10<br>2<br>0 0 1 1<br>-2 3 4 6

<strong>Output:</strong>
381
</pre>