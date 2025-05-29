<p>The electrical engineers�� indefatigable strive towards environmentally friendly energy production translated into the recent boom of hydro, solar, wind and geothermal power plants. While the production side seems ready, these ambitious projects have their bottleneck in the transportation and distribution: Besides the energy losses that occur during transportation over long distances, the renewable energy sources cannot provide power on demand �C they must be taken as provided by nature. Used at large scale in today��s networks, unreliable green energy can disrupt the balance of power grids easily and cause huge damage along with large-scale power outages.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="./22299/file/RXDX4AkC.png" alt="" width="705" height="234"></p>
<p>&nbsp;</p>
<p>Serious effort is thus put on researching transient and dynamic phenomena in power grids. You are offered a position in the lab for linear and planar distribution networks. Given a description of the distribution network��s line impedances Z<sub>i</sub> , you are to find the equivalent impedance between some couples of nodes. The knowledge of such equivalent impedances may speed up the network analysis considerably! Impedances are complex number whose real part represents the resistive line behaviour while the imaginary part stands for the capacitive (negative) or inductive (positive) characteristic. Lines are bidirectional, that is impedance(a,b) equals impedance (b,a).</p>
<p>It was proven that any linear and planar graph (can be drawn in a way that its edges intersect only at their endpoints) can be reduced into a single equivalent edge that represents the equivalent impedance between its ending nodes, using the following six transformations:</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="./22299/file/75aGcNUN.png" alt="" width="726" height="564"></p>
<p>&nbsp;</p>
<p>Now that you have all the necessary operations available, are you able to determine the equivalent impedance between several couples of nodes?</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases separated by an empty line. Each test-case starts with the number of nodes <em>N</em> (1&lt;=N&lt;=100), the number of bidirectional connections <em>C</em> (0&lt;=C&lt;=1000) and the number of equivalent impedances to compute <em>Z</em> (0&lt;=Z&lt;=10) on a line. Then follow <em>C </em>lines, each describing one bidirectional connection in the form <em>��EndPoint_1�� ��EndPoint_2�� ��Impedance��</em>. <em>��EndPoint_1��</em> <em>and ��EndPoint_2��</em> are in the range <em>1</em> to <em>N</em> and impedance has the format ��<em>re im</em>�� where <em>re </em>and <em>im</em> designate the real and imaginary parts respectively, both being real numbers <em>d</em> such that 10<sup>-3</sup> &lt; |d| &lt; 10<sup>3</sup>. The next <em>Z </em>lines each hold two integers, the indices of the nodes between which you are to compute the equivalent impedance. Input terminates on a test-case <em>with N=C=Z=0</em>, which must not be evaluated.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>For each couple of endpoints, output the equivalent impedance in the form ��<em>re im</em>�� where <em>re </em>and <em>im</em> designate the real and imaginary parts respectively. If the nodes are not connected, output ��no connection��. Electrical engineers will consider your result as correct if the absolute error on the real and imaginary parts is below 10<sup>-2</sup>. Finish each test-case on a blank line.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p><span style="font-family: courier new,courier;">5 10 3</span></p>
<p><span style="font-family: courier new,courier;">3 1 12.317 -0.779</span></p>
<p><span style="font-family: courier new,courier;">5 3 30.107 0.289</span></p>
<p><span style="font-family: courier new,courier;">5 1 27.447 -22.649</span></p>
<p><span style="font-family: courier new,courier;">4 2 15.351 24.371</span></p>
<p><span style="font-family: courier new,courier;">5 5 19.63 -3.549</span></p>
<p><span style="font-family: courier new,courier;">2 2 11.841 18.757</span></p>
<p><span style="font-family: courier new,courier;">4 5 4.834 -16.542</span></p>
<p><span style="font-family: courier new,courier;">3 5 5.022 -22.387</span></p>
<p><span style="font-family: courier new,courier;">2 5 24.768 -22.356</span></p>
<p><span style="font-family: courier new,courier;">5 2 27.351 12.053</span></p>
<p><span style="font-family: courier new,courier;">1 2</span></p>
<p><span style="font-family: courier new,courier;">2 3</span></p>
<p><span style="font-family: courier new,courier;">3 3</span></p>
<p><span style="font-family: courier new,courier;"><br></span></p>
<p><span style="font-family: courier new,courier;">10 10 4</span></p>
<p><span style="font-family: courier new,courier;">9 8 6.36 17.411</span></p>
<p><span style="font-family: courier new,courier;">1 3 27.596 -6.484</span></p>
<p><span style="font-family: courier new,courier;">9 10 4.735 -8.282</span></p>
<p><span style="font-family: courier new,courier;">8 8 6.901 27.939</span></p>
<p><span style="font-family: courier new,courier;">8 4 14.894 3.729</span></p>
<p><span style="font-family: courier new,courier;">5 4 14.311 -2.422</span></p>
<p><span style="font-family: courier new,courier;">10 10 11.009 6.225</span></p>
<p><span style="font-family: courier new,courier;">4 4 3.196 -32.703</span></p>
<p><span style="font-family: courier new,courier;">10 9 15.282 -14.799</span></p>
<p><span style="font-family: courier new,courier;">3 9 20.473 27.158</span></p>
<p><span style="font-family: courier new,courier;">10 9</span></p>
<p><span style="font-family: courier new,courier;">8 1</span></p>
<p><span style="font-family: courier new,courier;">2 9</span></p>
<p><span style="font-family: courier new,courier;">9 6</span></p>
<p>&nbsp;</p>
<p><strong>SAMPLE OUTPUT</strong></p>
<pre><span style="font-family: courier new,courier;">23.37 -7.26</span></pre>
<pre><span style="font-family: courier new,courier;">19.61 -6.97</span></pre>
<pre><span style="font-family: courier new,courier;">0.00 0.00</span></pre>
<pre><span style="font-family: courier new,courier;"><br></span></pre>
<pre><span style="font-family: courier new,courier;">3.79 -5.46</span></pre>
<pre><span style="font-family: courier new,courier;">54.43 38.09</span></pre>
<pre><span style="font-family: courier new,courier;">no connection</span></pre>
<pre><span style="font-family: courier new,courier;">no connection</span></pre>
<p style="text-align: center;"><span style="font-family: courier new,courier;"><img src="../../../content/imuteb:Elec2" alt="" width="224" height="163">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="../../../content/imuteb:Elec3" alt="" width="210" height="155"></span></p>
<p style="text-align: center;"><span style="font-family: courier new,courier;">Sample input 1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sample input 2<br></span></p>