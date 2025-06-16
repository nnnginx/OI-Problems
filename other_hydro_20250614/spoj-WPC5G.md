<p><span style="font-size: small;">It is emergency time! There has been a clash between the organizers of the Galactical Wars and the Inter-Galactic Parliament due to some feud. The entire civilization has been split into two groups A and B. The civilians in A love some particular members in the Organization Committee of the Galactical Wars, and hate some members from the Inter-Galactic Parliament. On the other hand, civilians in B love some particular members from the Inter-Galactic Parliament, and hate some in the Organization Committee.</span></p>
<p><span style="font-size: small;">You are Idli, the Inter-Galactic Dean, and it is your job to ensure satisfaction of the civilians. You decide to do so by impeaching some members from the Organization Committee and some from the Parliament. A civilian is satisfied if and only if all the members he loves are not impeached, and all the members he hates are impeached.</span></p>
<p><span style="font-size: small;">Of course, Idli wants to satisfy most number of civilians. Help Idli in devising an algorithm to do so.</span></p>
<p><span style="font-size: small;">&nbsp;</span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">First line contains two space separated integers n1 and n2, denoting the number of Galactic Wars organizers (numbered 1 to n1) and the number of Members of Parliaments(MP) respectively (numbered 1 to n2).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Second line contains a single integer ��n��, denoting the number of civilians.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">��n�� lines follow containing the description of the civilians in the following format:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">First character contains a single character ��A��, or ��B�� denoting the group of the civilian.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Then there is a space.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Then some space separated integers follow ended by -1 denoting the members of same group whom he loves. Then some space separated integers follow ended by -1 denoting the members of other group which he hates.&nbsp;</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">A single integer denoting the maximum number of civilians Idli can satisfy.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Constraints:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= n1 &lt;= 1000000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= n2 &lt;= 1000000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">1 &lt;= n &lt;= 500</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= number of organizers/MP a person loves &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">0 &lt;= number of organizers/MP a person hates &lt;= 50</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Example:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">4 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">A 1 -1 5 3 -1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">B 2 3 -1 2 5 -1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">B -1 -1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 36px; width: 1px; height: 1px; overflow: hidden;">Explanation: 3rd person doesn��t love or hate anyone, and thus is always satisfied. Only 1 out of the 1st 2 civilians can be satisfied. Hence Idli can satisfy at max 2 civilians.</div>
<p><strong>Input</strong>:</p>
<p>First line contains two space separated integers n1 and n2, denoting the number of Galactic Wars organizers (numbered 1 to n1) and the number of Members of Parliaments(MP) respectively (numbered 1 to n2).</p>
<p>Second line contains a single integer ��n��, denoting the number of civilians.</p>
<p>��n�� lines follow containing the description of the civilians in the following format:</p>
<p>First character contains a single character ��A��, or ��B�� denoting the group of the civilian.</p>
<p>Then there is a space.</p>
<p>Then some space separated integers follow ended by -1 denoting the members of same group whom he loves.</p>
<p>Then some space separated integers follow ended by -1 denoting the members of other group which he hates.&nbsp;</p>
<p>&nbsp;</p>
<p><strong>Output</strong>:</p>
<p>A single integer denoting the maximum number of civilians Idli can satisfy.</p>
<p>&nbsp;</p>
<p><strong>Constraints</strong>:</p>
<p>1 &lt;= n1 &lt;= 1000000</p>
<p>1 &lt;= n2 &lt;= 1000000</p>
<p>1 &lt;= n &lt;= 500</p>
<p>0 &lt;= number of organizers/MPs a person loves &lt;= 50</p>
<p>0 &lt;= number of organizers/MPs a person hates &lt;= 50</p>
<p>&nbsp;</p>
<p><strong>Time Limit</strong>: 1 second.</p>
<p>&nbsp;</p>
<p><strong>Example</strong>:</p>
<p><strong>Input</strong>:</p>
<p>5 5</p>
<p>3</p>
<p>A 1 -1 5 3 -1</p>
<p>B 2 3 -1 2 5 -1</p>
<p>B -1 -1</p>
<p>&nbsp;</p>
<p><strong>Output</strong>:</p>
<p>2</p>
<p>&nbsp;</p>
<p><strong>Explanation</strong>: 3rd person doesn��t love or hate anyone, and thus is always satisfied. Only 1 out of the 1st 2 civilians can be satisfied. Hence Idli can satisfy at max 2 civilians.</p>
<p>&nbsp;</p>