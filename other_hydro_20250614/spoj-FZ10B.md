<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/FZ10B/en/">English</a></td>
<td width="50%"><a href="/problems/FZ10B/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre><br><span style="white-space: normal;"><p style="font-family: Times; font-size: medium;">You may not hear about Nubulsa, an island country on the Pacific Ocean. Nubulsa is an undeveloped country and it is threatened by the rising of sea level. Scientists predict that Nubulsa will disappear by the year of 2012. Nubulsa government wants to host the 2011 Expo in their country so that even in the future, all the people in the world will remember that there was a country named ``Nubulsa".</p>
<p style="font-family: Times; font-size: medium;">As you know, the Expo garden is made up of many museums of different countries. In the Expo garden, there are a lot of bi-directional roads connecting those museums, and all museums are directly or indirectly connected with others. Each road has a tourist capacity which means the maximum number of people who can pass the road per second.</p>
<p style="font-family: Times; font-size: medium;">Because Nubulsa is not a rich country and the ticket checking machine is very expensive, the government decides that there must be only one entrance and one exit. The president has already chosen a museum as the entrance of the whole Expo garden, and it's the Expo chief directory Wuzula's job to choose a museum as the exit.</p>
<p style="font-family: Times; font-size: medium;">Wuzula has been to the Shanghai Expo, and he was frightened by the tremendous ``people mountain people sea" there. He wants to control the number of people in his Expo garden. So Wuzula wants to find a suitable museum as the exit so that the ``max tourists flow" of the Expo garden is the minimum. If the ``max tourist flow" is&nbsp;<em>W</em>, it means that when the Expo garden comes to ``stable status", the number of tourists who enter the entrance per second is at most<em>W</em>. When the Expo garden is in ``stable status", it means that the number of people in the Expo garden remains unchanged.</p>
<p style="font-family: Times; font-size: medium;">Because there are only some posters in every museum, so Wuzula assume that all tourists just keep walking and even when they come to a museum, they just walk through, never stay.</p>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<h1><span style="color: #ff0000; font-size: small;"><span style="font-size: medium;"><span style="font-family: 'comic sans ms', sans-serif;">Input</span></span></span></h1>
<p style="font-family: Times; font-size: medium;">There are several test cases, and the input ends with a line of ``<tt>0 0 0</tt>".</p>
<p style="font-family: Times; font-size: medium;">For each test case:</p>
<p style="font-family: Times; font-size: medium;">The first line contains three integers&nbsp;<em>N</em>,&nbsp;<em>M</em>&nbsp;and&nbsp;<em>S</em>, representing the number of the museums, the number of roads and the No. of the museum which is chosen as the entrance (all museums are numbered from 1 to&nbsp;<em>N</em>). For example,&nbsp;<tt>5 5 1</tt>&nbsp;means that there are 5 museums and 5 roads connecting them, and the No. 1 museum is the entrance.</p>
<p style="font-family: Times; font-size: medium;">The next&nbsp;<em>M</em>&nbsp;lines describe the roads. Each line contains three integers&nbsp;<em>X</em>,&nbsp;<em>Y</em>&nbsp;and&nbsp;<em>K</em>, representing the road connects museum&nbsp;<em>X</em>&nbsp;with museum&nbsp;<em>Y</em>&nbsp;directly and its tourist capacity is&nbsp;<em>K</em>.</p>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<p style="font-family: Times; font-size: medium;"><br>Please note:</p>
<p style="font-family: Times; font-size: medium;">1 &lt;&nbsp;<em>N ��&nbsp;</em>300,&nbsp;0 &lt;&nbsp;<em>M&nbsp;<span style="font-family: Times; font-size: medium; font-style: italic;">��&nbsp;</span></em>50000,&nbsp;0 &lt;&nbsp;<em>S</em>,&nbsp;<em>X</em>,&nbsp;<em>Y</em><em>&nbsp;<span style="font-family: Times; font-size: medium; font-style: italic;">��</span><span style="font-family: Times; font-size: medium; font-style: italic;">&nbsp;</span></em><em>N</em>,&nbsp;0 &lt;&nbsp;<em>K&nbsp;<span style="font-family: Times; font-size: medium; font-style: italic;">��&nbsp;</span></em>1000000</p>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<h1><span style="color: #ff0000;"><span style="font-size: medium;"><span style="font-family: 'comic sans ms', sans-serif;">Output</span></span></span></h1>
<p style="font-family: Times; font-size: medium;">For each test case, print a line with only an integer&nbsp;<em>W</em>, representing the ``max tourist flow" of the Expo garden if Wuzula makes the right choice.</p>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<h1><span style="color: #ff0000; font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;">Sample Input</span></span></h1>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<pre>5 5 1 
1 2 5 
2 4 6 
1 3 7 
3 4 3 
5 1 10 
0 0 0
</pre>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<h2 style="font-family: Times;"><span style="color: #ff0000; font-size: small;"><span style="font-family: 'comic sans ms', sans-serif;">Sample Output</span></span></h2>
<p style="font-family: Times; font-size: medium;">&nbsp;</p>
<pre>8</pre>
</span></pre>
<p> </p>