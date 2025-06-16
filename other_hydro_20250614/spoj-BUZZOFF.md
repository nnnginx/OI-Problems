<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">BUZZ OFF</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Commander Nebula decided to take interns into Star Command to join the Little Green Men (LGMs). And the job of physical training of these LGMs went to Buzz Lightyear. Assume N interns are taken, each with a distinct LGM ID.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Being buzy with XR, Buzz sent Mira Nova to select a few of the interns and line them in the training center. XR noticed that he neither told Mira how many LGMs to select, nor in which order to arrange them; so Mira can select any number M of students (1&lt;=M&lt;=N) and line them up randomly (Assume that if Mira is to select M LGMs, then she selects the M smallest LGM IDs, eg, if N=5 and IDs be 12,3,4,11,2 and she decided to select 3 LGMs, then she picks up 3,4 and 2).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">XR wonders, how many different arrangements might Buzz find on arriving in the training centre for which no LGM is more than unit distance away from its correct position, and Buzz has to do less work in ordering them correctly (in increasing order of LGM ID).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">As result might be large, output result modulo 10^9+7 (1000000007)</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">INPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">first line contains T, number of test cases</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Next T lines contain single number N, indicating number of LGM interns.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">OUTPUT:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">T lines, each with the answer for corresponding case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CONSTRAINTS:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=T&lt;=10^5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1&lt;=N&lt;=10^18</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EXAMPLE:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Input:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">8</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">10</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Output:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">1</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">19</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">87</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">231</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Explaination:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for N=1, only case is to pick the only LGM</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">for N=2, and LGM IDs are say 1 and 2, then Buzz might find [1], [1,2], or [2,1] Therefore 3</div>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>BUZZ OFF</p>
<p>Commander Nebula decided to take interns into Star Command to join the Little Green Men (LGMs). And the job of physical training of these LGMs went to Buzz Lightyear. Assume N interns are taken, each with a distinct LGM ID.</p>
<p>Being busy with XR, Buzz sent Mira Nova to select a few of the interns and line them in the training center. XR noticed that he neither told Mira how many LGMs to select, nor in which order to arrange them; so Mira can select any number M of students (1&lt;=M&lt;=N) and line them up randomly (Assume that if Mira is to select M LGMs, then she selects the M smallest LGM IDs, eg, if N=5 and IDs be 12,3,4,11,2 and she decided to select 3 LGMs, then she picks up 3,4 and 2).</p>
<p>XR wonders, how many different arrangements might Buzz find on arriving in the training centre for which no LGM is more than unit distance away from its correct position, and Buzz has to do less work in ordering them correctly (in increasing order of LGM ID).</p>
<p>As result might be large, output result modulo 10^9+7 (1000000007)</p>
<p>&nbsp;</p>
<p>INPUT:</p>
<p>first line contains T, number of test cases</p>
<p>Next T lines contain single number N, indicating number of LGM interns.</p>
<p>&nbsp;</p>
<p>OUTPUT:</p>
<p>T lines, each with the answer for corresponding case.</p>
<p>&nbsp;</p>
<p>CONSTRAINTS:</p>
<p>1&lt;=T&lt;=10^4</p>
<p>1&lt;=N&lt;=10^18</p>
<p>&nbsp;</p>
<p>EXAMPLE:</p>
<p>Input:</p>
<p>5</p>
<p>1</p>
<p>2</p>
<p>5</p>
<p>8</p>
<p>10</p>
<p>&nbsp;</p>
<p>Output:</p>
<p>1</p>
<p>3</p>
<p>19</p>
<p>87</p>
<p>231</p>
<p>&nbsp;</p>
<p>Explaination:</p>
<p>for N=1, only case is to pick the only LGM</p>
<p>for N=2, and LGM IDs are say 1 and 2, then Buzz might find [1], [1,2], or [2,1] Therefore 3</p>
<p>&nbsp;</p>