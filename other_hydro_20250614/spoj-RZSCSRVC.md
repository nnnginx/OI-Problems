<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">You all know about famous secret service agent Masud Rana. Masud Rana is a fictional</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">character created in 1966 by writer Qazi Anwar Hussain.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Today he is going to send a message to his colleague Shohana Chowdhury in encrypted format.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">He likes letter ¡®R¡¯ very much, so he encrypt a massage s in following pattern with height h</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">(always odd):</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">If his massage is s = ¡°ABCDEFGHIJKLMNOPQRSTUVWXYZ¡± &amp;amp; h = 5</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">Then his message will be like this:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">EFG#RST</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">D#H#Q#U</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">CJI#PWV</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">BK##OX</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A#LMN#YZ</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">That¡¯s mean result format have height h=5, and all letter will be in sequentially make big ¡®R¡¯. All</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">other space will be fill up with ¡®#¡¯. Please see the following figure for better understanding.</div>
<p>You all know about famous secret service agent <strong>Masud Rana</strong>. Masud Rana is a fictional character created in 1966 by writer <strong>Qazi Anwar Hussain</strong>. Today he is going to send a message to his colleague <strong>Shohana Chowdhury</strong> in encrypted format.</p>
<p>He likes letter <em><strong>R</strong></em> very much, so he encrypt a massage s in following pattern with height <strong>h</strong>(always odd).</p>
<p>If his massage is s = ¡°ABCDEFGHIJKLMNOPQRSTUVWXYZ¡± &amp; h = 5</p>
<p>Then his message will be like this:</p>
<p style="text-align: left;">EFG#RST</p>
<p style="text-align: left;">D#H#Q#U</p>
<p style="text-align: left;">CJI#PWV</p>
<p style="text-align: left;">BK##OX</p>
<p style="text-align: left;">A#LMN#YZ</p>
<p>That¡¯s mean result format have height h=5, and all letter will be in sequentially make big <strong>R</strong>. All other space will be fill up with <strong>#</strong>. Please see the following figure for better understanding.</p>
<p><img src="../../../../../../content/simes:RZSCSRVC.jpg">&nbsp;</p>
<p>(Line has drawn for explanatatory purpose )</p>
<h3>Input</h3>
<p>In first there is two integer <strong>n</strong> (1 &lt;= n &lt;= 1000) and <strong>h</strong>(1 &lt;= h &lt;=n, h is <strong>odd</strong>), length of the message and height of output. In next line there is a message <strong>s</strong>, message is a non-empty string consist with only <strong>capital letter</strong>.</p>
<h3>Output</h3>
<p>Print h line with corresponding answer with describe format. <strong>&nbsp;</strong></p>
<p><strong>Note that, there should not have any extra # after last letter of each line.</strong></p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
13 3
PHQGHUMEAYLNA

<strong>Output:</strong>
QG#YL
HH#AN
PUMEA</pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
22 5
MXWTPTTTYKDUYVXJBZHQUP

<strong>Output:</strong>
PTT#ZHQ
T#T#B#U
WKY#J#P
XD##X
M#UYV</pre>
<h3>Example 3</h3>
<pre><strong>Input:</strong>
22 7
MXWTPTTTYKDUYVXJBZHQUP

<strong>Output:</strong>
TTYK
T##D
P##U
TXVY
WJ###P
X#B##U
M##ZHQ</pre>
<pre>[ This problem originally contributed by <strong>Reajul Haque Reayz, CSE, CoU</strong> ]</pre>