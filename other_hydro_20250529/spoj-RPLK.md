<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">&nbsp;Giselle is working on her house, as her husband won't be able to help in the task, she gently asks you for help, the task is very simple, Giselle wants to build some stairs that communicate two floors in the house, the stairs will be made of W segments of wooden, she is very confident on building the stairs, but she wants to build the stairs with some separation between steps. As you know, the end of a step is overlapped by the beginning of the other, and so on, between steps there are a single separation, as Giselle is very conservative, she wants to build the stairs using at most W segments of wood.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> The next image will help you to understand the task</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> </span></p>
<p><img src="../../../../../../content/simes:rplk.png" border="0"></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> As you can see in the image, there is a single separation between each step relating to the height and the width of every step.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Giselle wants to build stairs using E pieces of wood that she wants to cut into at most W steps. You can only cut vertically and can't rotate the given pieces. Each step's width must be exactly M+1. M is the overlap and 1 is a constant width left placing feet.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>INPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> The first line of the test data will start with an integer T representing the T test cases, then, T cases will follow.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> Each case starts with four positive integers (E,M,K,W) denoting E pieces of wood, M meters of overlap, K height of separator between each step and W, the maximum number of steps that can be cut out. Next, E lines will follow, each with two integers Eh and Ew representing respectively the height and the width of each piece of wood Giselle has.</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>OUTPUT:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"> You must output the string ��Scenario #i: �� where i is the number of test case you're analyzing (starting by 1), followed by the maximum amount of height that you can possibly build</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<table style="width: 100%;" border="0" cellspacing="0" cellpadding="4">
<colgroup><col width="128*"> <col width="128*"> </colgroup> 
<tbody>
<tr valign="TOP">
<td style="border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="CENTER"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>INPUT</strong></span></p>
</td>
<td style="border: 1px solid #000000; padding: 0.04in;" width="50%">
<p align="CENTER"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>OUTPUT</strong></span></p>
</td>
</tr>
<tr valign="TOP">
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in;" width="50%">
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">5 1 1 3</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">6 2</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">5 10</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">4 20</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 15</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 1</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 1 0 5</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">3 15</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 20</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">1 60</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">2 1 1 25</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">15 10</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">12 10</span></p>
</td>
<td style="border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in;" width="50%">
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#1: 19</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#2: 15</span></p>
<p align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Scenario 			#3: 145</span></p>
</td>
</tr>
</tbody>
</table>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">Explanation of the first case:</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">You can only cut the segment of width 6 into one piece, but the 5 segment of width 10 you can cut it into 5 pieces, as you only need 3 pieces to use, the maximum height will be of 6+5+5+3 = 19</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><strong>CONSTRAINTS:</strong></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;">(1 &lt;= Width and Height of each wooden piece &lt;= 1000) = WiHi</span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;">Small input (40%)</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1&lt;= T &lt;=200</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1&lt;= {E,K,M} &lt;=100</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> WiHi &lt;= M &lt;= 100</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1&lt;= W &lt;=100</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY">&nbsp;</p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;">Large Input (60%)</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1&lt;= T &lt;=10</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1&lt;= {E,K} &lt;=100,000</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> WiHi &lt;= M &lt;= 1,000</span></span></p>
<p style="margin-bottom: 0in;" align="JUSTIFY"><span style="font-family: 'Liberation Sans', sans-serif;"><span style="font-size: small;"> 1 &lt;= W &lt;= 10,000</span></span></p>