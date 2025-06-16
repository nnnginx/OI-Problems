<p><strong>Background</strong></p>
<p>Hippo and his two friends lost their path in a jungle. In this days jungle is most dangerous place. The jungle has lots of tunnels. Also there lived some brutal animals in the dangerous zone(the cell ¡®D¡¯). Now Hippo and his two friends want to go to safe places(¡®#¡¯) as fast as possible i.e. in minimum times.</p>
<p><strong>Problem</strong></p>
<p>In this problem you are given the jungle-map as a grid. Where ¡®A¡¯,¡¯B¡¯,¡¯C¡¯ denotes the position of Hippo and his two friends. ¡¯D¡¯ indicates dangerous place. No one can stay this cell.&nbsp; ¡®#¡¯ denotes the safe place. In this grid there are also given some characters (E-Z) which occur more than one and donates if one reaches a tunnel he can go any other tunnel of same character and also any adjacent cell(8-directions). They also can move any adjacent cell from ordinary place. Each move takes 1 unit of time. Is it possible to go all of them to safe places??&nbsp; If possible then what is the minimum time required.<strong>&nbsp;</strong></p>
<p><strong>Input</strong></p>
<p>Input starts with an integer&nbsp;<strong>T (¡Ü 15)</strong>, denoting the number of test cases.</p>
<p>Each case starts with a line containing two positive integers&nbsp;<strong>H</strong>&nbsp;and&nbsp;<strong>W</strong>;&nbsp;<strong>W</strong>&nbsp;and&nbsp;<strong>H</strong>&nbsp;are the numbers of cells in the&nbsp;<strong>x</strong>&nbsp;and&nbsp;<strong>y</strong>&nbsp;directions, respectively.&nbsp;<strong>W</strong>&nbsp;and&nbsp;<strong>H</strong>&nbsp;are not more than 20. There will be&nbsp;<strong>H</strong>&nbsp;more lines in the data set, each of which includes&nbsp;<strong>W</strong>&nbsp;characters. Each character represents the status of a cell as follows.</p>
<p>1)&nbsp;<strong>'.'</strong>&nbsp;¨C ordinary place.</p>
<p>2)&nbsp;<strong>'#'</strong>&nbsp;¨C safe place</p>
<p>3)&nbsp;<strong>'A', 'B','C'</strong>&nbsp;- initial position of Hippo and his friends.</p>
<p>4)&nbsp;<strong>'D'</strong>&nbsp;¨C Dangerous place.</p>
<p>3)&nbsp;<strong>'E-Z'</strong>&nbsp;- denote the tunnel.</p>
<p><strong>Output</strong></p>
<p>For each test case, print the case number and minimum time if it is not possible to reach all of them into safe position otherwise print ¡°impossible¡± without quote.</p>
<table border="0" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="319" valign="top">
<p><strong>Sample Input</strong></p>
</td>
<td width="319" valign="top">
<p><strong>Output for Sample Input</strong></p>
</td>
</tr>
<tr>
<td width="319" valign="top">
<p>2</p>
<p>&nbsp;</p>
<p>5   6</p>
<p>C..E#.<br>.D....<br>F..E..<br>.D..A.<br>.B.D.F</p>
<p>&nbsp;</p>
<p>4 &nbsp;4<br>C.D#<br>.FDD<br>A..E<br>.B.F</p>
</td>
<td width="319" valign="top">
<p>Case 1: 4<br>Case 2: impossible</p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>