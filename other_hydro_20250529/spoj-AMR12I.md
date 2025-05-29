<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'"For I am Saruman the Wise, Saruman Ring-maker, Saruman of Many Colours!"</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">'I looked then and saw that his robes, which had seemed white, were not so, but were woven of all colours. And if he moved they shimmered and changed hue so that the eye was bewildered.' - Gandalf the Grey.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">And so it was that Saruman decided to brand his Uruk-hai army with the many colours that he fancied. His method of branding his army was as follows.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">He straps his army of N Uruk-hai onto chairs on a conveyor belt. This conveyor belt passes through his colouring-room, and can be moved forward or backward. The Uruk-hai are numbered 0 to N-1 according to the order in which they are seated. Saruman wishes that the i'th Uruk-hai be coloured with the colour c[i].</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Further, his colouring-room has space for exactly K chairs. Once the chosen K consecutive Uruk-hai are put into the room, a colour jet sprays all K of them with any fixed colour. The conveyor belt is not circular (which means that the N-1'th and the 0'th Uruk-hai are not consecutive). Note that Uruk-hai can be recoloured in this process.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Saruman wants to find out what is the minimum number of times that the jet needs to be used in order to colour his army in the required fashion. If it is not possible to colour the army in the required fashion, output -1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input (STDIN):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The first line contains the number of test-cases T.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Each test case consists of 2 lines. The first line contains two space-separated integers, N and K.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">This is followed by a single like containing a string of length N, describing the colours of the army. The i'th character of the string denotes the colour of the i'th Uruk-hai in the army.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output (STDOUT):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output T lines, one for each test case containing the answer for the corresponding test case. Remember if it is not possible to colour the army as required, output -1.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= T &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= K &lt;= N &lt;= 20,000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">The string c has length exactly N and contains only the characters 'a',...,'z'.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">rgg</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3 3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">rgg</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Sample Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">-1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Notes/Explanation of Sample Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the first test case, soldiers 0 and 1 can first be painted with 'r', and then soldiers 1 and 2 can be painted with 'g'.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the second test case, since N = K, all the soldiers will only have the same color.</div>
<p>&nbsp;</p>
<p>'"For I am Saruman the Wise, Saruman Ring-maker, Saruman of Many Colours!"</p>
<p>'I looked then and saw that his robes, which had seemed white, were not so, but were woven of all colours. And if he moved they shimmered and changed hue so that the eye was bewildered.' - Gandalf the Grey.</p>
<p>And so it was that Saruman decided to brand his Uruk-hai army with the many colours that he fancied. His method of branding his army was as follows.</p>
<p>He straps his army of N Uruk-hai onto chairs on a conveyor belt. This conveyor belt passes through his colouring-room, and can be moved forward or backward. The Uruk-hai are numbered 0 to N-1 according to the order in which they are seated. Saruman wishes that the i'th Uruk-hai be coloured with the colour c[i].</p>
<p>Further, his colouring-room has space for exactly K chairs. Once the chosen K consecutive Uruk-hai are put into the room, a colour jet sprays all K of them with any fixed colour. The conveyor belt is not circular (which means that the N-1'th and the 0'th Uruk-hai are not consecutive). Note that Uruk-hai can be recoloured in this process.</p>
<p>&nbsp;</p>
<p>Saruman wants to find out what is the minimum number of times that the jet needs to be used in order to colour his army in the required fashion. If it is not possible to colour the army in the required fashion, output -1.</p>
<p>&nbsp;</p>
<p><strong>Input (STDIN):</strong></p>
<p>The first line contains the number of test-cases T.</p>
<p>Each test case consists of 2 lines. The first line contains two space-separated integers, N and K.</p>
<p>This is followed by a single like containing a string of length N, describing the colours of the army. The i'th character of the string denotes the colour of the i'th Uruk-hai in the army.</p>
<p>&nbsp;</p>
<p><strong>Output (STDOUT):</strong></p>
<p>Output T lines, one for each test case containing the answer for the corresponding test case. Remember if it is not possible to colour the army as required, output -1.</p>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>
<p>1 &lt;= T &lt;= 50</p>
<p>1 &lt;= K &lt;= N &lt;= 20,000</p>
<p>The string c has length exactly N and contains only the characters 'a',...,'z'.</p>
<p>&nbsp;</p>
<p><strong>Sample Input:</strong></p>
<p>2</p>
<p>3 2</p>
<p>rgg</p>
<p>3 3</p>
<p>rgg</p>
<p>&nbsp;</p>
<p><strong>Sample Output:</strong></p>
<p>2</p>
<p>-1</p>
<p>&nbsp;</p>
<p><strong>Notes/Explanation of Sample Input:</strong></p>
<p>In the first test case, soldiers 0 and 1 can first be painted with 'r', and then soldiers 1 and 2 can be painted with 'g'.</p>
<p>In the second test case, since N = K, all the soldiers will only have the same color.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>