<p id="docs-internal-guid-6ca5b52c-4c4f-b50c-b4d5-72cdc37863b6" style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;text-align: justify;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Integer X is Square-Free if and only if p</span><span style="font-size:9px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:super;">2</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> (p is prime) does not divide it. For example, 15 is a square-free number but 12 isn't, because 2</span><span style="font-size:9px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:super;">2</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> = 4 is one of its divisors.</span></p>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;text-align: justify;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Write a program that outputs whether the product of two numbers is a square-free number.</span></p>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:bold;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Input</span></p>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">The first line contains T (1 ¡Ü T ¡Ü 100), the number of test cases. T lines follow, one per test case. Each of these lines contain two integers </span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:italic;font-variant:normal;text-decoration:none;vertical-align:baseline;">a</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> and </span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:italic;font-variant:normal;text-decoration:none;vertical-align:baseline;">b</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> (1 ¡Ü a, b ¡Ü 10</span><span style="font-size:9px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:super;">18</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">). </span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:bold;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">a and b are NOT necessarily square-free.</span></p>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:bold;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Output</span></p>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Per test case:</span></p>
<p>&nbsp;</p>
<ul style="margin-top:0pt;margin-bottom:0pt;">
<li style="list-style-type:disc;font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;" dir="ltr">
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Output a single line containing "YES" if the product of </span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:italic;font-variant:normal;text-decoration:none;vertical-align:baseline;">a</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> and </span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:italic;font-variant:normal;text-decoration:none;vertical-align:baseline;">b</span><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;"> is square-free, or "NO" otherwise. In any case, do not include quotes in your output.</span></p>
</li>
</ul>
<p>&nbsp;</p>
<p style="line-height:1.15;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:bold;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Sample cases</span></p>
<p>&nbsp;</p>
<div style="margin-left:0pt;" dir="ltr">
<table style="border:none;border-collapse:collapse" border="0">
<colgroup><col width="623"></colgroup> 
<tbody>
<tr style="height: 0px;">
<td style="border-left:solid #000000 1px;border-right:solid #000000 1px;border-bottom:solid #000000 1px;border-top:solid #000000 1px;vertical-align:top;padding:7px 7px 7px 7px">
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Input</span></p>
</td>
</tr>
<tr style="height: 0px;">
<td style="border-left:solid #000000 1px;border-right:solid #000000 1px;border-bottom:solid #000000 1px;border-top:solid #000000 1px;vertical-align:top;padding:7px 7px 7px 7px">
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">4</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">1 1</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">6 13</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">10 2</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">12 1</span></p>
</td>
</tr>
<tr style="height: 0px;">
<td style="border-left:solid #000000 1px;border-right:solid #000000 1px;border-bottom:solid #000000 1px;border-top:solid #000000 1px;vertical-align:top;padding:7px 7px 7px 7px">
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">Output</span></p>
</td>
</tr>
<tr style="height: 0px;">
<td style="border-left:solid #000000 1px;border-right:solid #000000 1px;border-bottom:solid #000000 1px;border-top:solid #000000 1px;vertical-align:top;padding:7px 7px 7px 7px">
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">YES</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">YES</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">NO</span></p>
<p style="line-height:1;margin-top:0pt;margin-bottom:0pt;" dir="ltr"><span style="font-size:15px;font-family:Arial;color:#000000;background-color:transparent;font-weight:normal;font-style:normal;font-variant:normal;text-decoration:none;vertical-align:baseline;">NO</span></p>
</td>
</tr>
</tbody>
</table>
</div>