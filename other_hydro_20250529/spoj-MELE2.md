<p>   </p>

<table class="problems" style="width: 100%; background-color: #ee7b10;" border="0">
<tbody>
<tr class="navigation">
<td style="text-align: center;" width="50%"><a href="/problems/MELE2/en/">English</a></td>
<td style="text-align: center;" width="50%"><a href="/problems/MELE2/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<pre>Edward works as an engineer for Non-trivial Elevators: Engineering, <br>Research and Construction (NEERC). His new task is to design a brand new <br>elevator for a skyscraper with h ﬂoors.<br>Edward has an idee ﬁxe: he thinks that four buttons are enough to control<br>the movement of the elevator.<br>His last proposal suggests the following four buttons:<br>• Move a ﬂoors up.<br>• Move b ﬂoors up.<br>• Move c ﬂoors up.<br>• Return to the ﬁrst ﬂoor.<br>Initially, the elevator is on the ﬁrst ﬂoor. A passenger uses the ﬁrst <br>three buttons to reach the ﬂoor she needs. If a passenger tries to move <br>a, b or c ﬂoors up and there is no such ﬂoor (she attempts to move<br>higher than the h-th ﬂoor), the elevator doesn’t move.<br>To prove his plan worthy, Edward wants to know how many ﬂoors are actually <br>accessible from the ﬁrst ﬂoor via his elevator. Help him calculate this number.<br></pre>
<h3>Input</h3>
<pre>TThe ﬁrst line of the input ﬁle contains one integer h — the height of <br>the skyscraper (1 ≤ h ≤ 10^18).<br>The second line contains three integers a, b and c — the parameters of <br>the buttons (1 ≤ a, b, c ≤ 100000)<br><br>SAMPLE INPUT 1<br>15<br>4 7 9<br><br>SAMPLE INPUT 2<br>500000<br>160 96 111<br><br>SAMPLE INPUT 3<br>987654321987654321<br>99995 99997 99999<br><br></pre>
<h3>Output</h3>
<pre> <br>Output one integer number — the number of ﬂoors that are reachable from <br>the ﬁrst ﬂoor<br><br>SAMPLE OUTPUT 1<br>9<br>SAMPLE OUTPUT 2<br>498167<br>SAMPLE OUTPUT 3<br>987654319487854318<br></pre>
<p> </p>