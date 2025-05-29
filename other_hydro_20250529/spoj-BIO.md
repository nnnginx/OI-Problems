<p>It was no later than 1869 that Jules Verne succeeded to vulgarize interest in the depths of the oceans through his science-fiction novel ��Twenty thousand leagues under the sea��. On board the Nautilus manoeuvred by captain Nemo, the crew visits the lost city of Atlantis and gets to know strangest kinds of sea dwellers.</p>
<p>Nearly a century later, one of the deepest points on Earth, the Challenger Deep was visited by Piccard and Walsh and a Swiss flag was dibbled at 10��924 metres below sea level. The ridership of the Trieste submarine was amazed by the animal life in these depths.</p>
<p>&nbsp;</p>
<p style="text-align: center;"><img src="../../../content/imuteb:biology1" alt="" width="510" height="340"></p>
<p>&nbsp;</p>
<p>Recently a team of biologists decided to investigate these depths of the Mariana Trench and especially their So Weird Exotic Rare Citizens (SWERC). To this goal a preliminary study was performed, which showed that the species in the Mariana Trench have very local biotopes, which if projected onto the sea surface, can be described by convex polygons. All the biotopes are located at the same depth and some may overlap. The biologists now want to install racks and cameras in each biotope in order to attract and film them. As delicious as the food at the racks might be, no species would ever take the risk to transgress the borders of its habitat. As these cameras and the associated telecommunication system are extremely expensive, their number is to be minimized. Can you tell the biologists for how many cameras they need to account in their budget planning in order not to miss any species if they choose the locations in a clever way? You may consider each camera-rack couple as a mathematical point which must lie <span style="text-decoration: underline;">strictly</span> inside the biotope in order to attract the related species.</p>
<p>&nbsp;</p>
<p><strong>INPUT</strong></p>
<p>The input consists of several test-cases separated by an empty line. Each test-case starts with the number of species <em>S (0&lt;=S&lt;=20) </em>. Each of the next<em> S</em> lines describes one biotope. The first entry indicates the number <em>n<sub>i</sub></em> &nbsp;of vertices of the convex polygon. Then follow their coordinates in the order <em>x1 y1 x2 y2 ... xn<sub>i</sub> yn<sub>i</sub></em> <em>(|xi|,|yi|&lt;=1000)</em>. Input terminates on a test-case <em>with S=0</em>, which must not be evaluated.</p>
<p>&nbsp;</p>
<p><strong>OUTPUT</strong></p>
<p>For each test-case, output the minimum number of camera-rack couples necessary to screen all the species listed in the input.</p>
<p>&nbsp;</p>
<p><strong>SAMPLE INPUT</strong></p>
<p>3</p>
<p>3 11.00 0.00 -2.50 7.79 -2.50 -7.79</p>
<p>4 4.00 -3.00 -3.00 4.00 -10.00 -3.00 -3.00 -10.00</p>
<p>4 4.00 2.00 3.00 3.00 2.00 2.00 3.00 1.00</p>
<p>&nbsp;</p>
<p>10</p>
<p>7 -317.00 99.00 -330.55 127.15 -361.01 134.10 -385.43 114.62 -385.43 83.38 -361.01 63.90 -330.55 70.85</p>
<p>6 -99.00 93.00 -238.50 334.62 -517.50 334.62 -657.00 93.00 -517.50 -148.62 -238.50 -148.62</p>
<p>4 113.00 -134.00 42.00 -63.00 -29.00 -134.00 42.00 -205.00</p>
<p>3 90.00 -68.00 -261.00 134.65 -261.00 -270.65</p>
<p>7 218.00 -342.00 147.22 -195.02 -11.83 -158.71 -139.38 -260.43 -139.38 -423.57 -11.83 -525.29 147.22 -488.98</p>
<p>6 131.00 -286.00 38.00 -124.92 -148.00 -124.92 -241.00 -286.00 -148.00 -447.08 38.00 -447.08</p>
<p>4 -170.00 -247.00 -172.00 -245.00 -174.00 -247.00 -172.00 -249.00</p>
<p>4 -332.00 -102.00 -395.00 -39.00 -458.00 -102.00 -395.00 -165.00</p>
<p>6 -52.00 -224.00 -196.50 26.28 -485.50 26.28 -630.00 -224.00 -485.50 -474.28 -196.50 -474.28</p>
<p>5 -101.00 163.00 -210.87 314.22 -388.63 256.46 -388.63 69.54 -210.87 11.78</p>
<p>&nbsp;</p>
<p>0</p>
<p><span style="font-family: courier new,courier;">&nbsp;</span></p>
<p><strong>SAMPLE OUTPUT</strong></p>
<p>2</p>
<p>5</p>
<p>&nbsp;</p>
<p><img src="../../../content/imuteb:biology2" alt="" width="256" height="243"> &nbsp; &nbsp;&nbsp; <img src="../../../content/imuteb:biology3" alt="" width="302" height="239"></p>
<p style="text-align: left;">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sample input 1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sample input 2</p>