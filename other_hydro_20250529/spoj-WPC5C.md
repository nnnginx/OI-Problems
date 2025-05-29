<p><span id="docs-internal-guid-617ee771-0f8f-0da0-b16b-81932335f359"> </span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">It is 2048, and a Martian robot called SSH3 wants to win galactical wars, as he does every year.</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; white-space: pre-wrap; line-height: 1.15;"><span style="font-size: small;">He has been chosen to participate in the prestigious Sword Game, possibly the last one to ever happen. This is the format of the Sword Game.</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><span style="background-color: transparent; white-space: pre-wrap; line-height: 1.15;">Every sword has a name S which is a string of n characters from a-z. </span><span style="background-color: transparent; white-space: pre-wrap; line-height: 1.15;">The strength of the sword is decided in the following way.</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">Define a function f (l1, l2) for every 1&lt;= l1, l2 &lt;= n. Find all the substrings of the sword name S with length l1. Then, ind1 is the index such that it is the lexicographically smallest among these l1 length substrings. (If there are multiple such substrings, then we consider the <strong>lower</strong> index).</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">Similarly, ind2 is defined. Then, f (l1, l2) = |ind1 - ind2|. (All indices are 0-based)</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">Strength (S) = (Expected Value (f)), over all l1, l2.</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">As a Martian, SSH3 is also expected to be very good at Maths. He is asked to find out the strength of the sword. But as all other Martians, he has come from the city of Quoda, where everybody is pathetic at Maths. Hence, he asks you to help him. Ouput the value of n^2 * Strength (S).</span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;"><br></span></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Input:</strong>&nbsp;</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">First line contains the integer n.</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">Second line contains the name of the sword S.</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><strong><span style="font-size: small;">Output:&nbsp;</span></strong></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">A single line containing an <strong>Integer</strong>, that is the value of n^2 * Strength (S).</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><strong><span style="font-size: small;">Constraints:</span></strong></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">1 &lt;= n &lt;= 100000</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">S contains exactly n characters from ��a�� to ��z��.</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Time Limit</strong>: 8 seconds.</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Examples</strong>:</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Input</strong>:</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">2&nbsp;</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">ab</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Output</strong>:</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">0</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><strong>Explanation</strong>: f(l1,l2) can take one of the following 4 values:</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">f(1,1) = 0 ( ind1 = 0, ind2 = 0 )</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">f(1,2) = 0 ( ind1 = 0, ind2 = 0 )</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">f(2,1) = 0 ( ind1 = 0, ind2 = 0 )</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">f(2,2) = 0 ( ind1 = 0, ind2 = 0 )</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">E(f(l1,l2)) = 0</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;">2^2 * E(f(l1,l2)) = 0</span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="font-size: small;"><br></span></p>
<p style="line-height: 1.15; margin-top: 0pt; margin-bottom: 0pt;" dir="ltr"><span style="background-color: transparent; vertical-align: baseline; white-space: pre-wrap;"><span style="font-size: small;">&nbsp;</span></span></p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Input:&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">First line contains the integer n.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Second line contains the name of the sword S.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Output:&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">A single line containing an INTEGER, that is the value of n^2 * Strength (S).</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Constraints:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">1 &lt;= n &lt;= 100000</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">S contains exactly n characters from ��a�� to ��z��.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Time Limit: 8 seconds.</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Examples:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Input:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2&nbsp;</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">ab</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Output:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">0</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">Explanation: f(l1,l2) can take one of the following 4 values:</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">f(1,1) = 0 ( ind1 = 0, ind2 = 0 )</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">f(1,2) = 0 ( ind1 = 0, ind2 = 0 )</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">f(2,1) = 0 ( ind1 = 0, ind2 = 0 )</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">f(2,2) = 0 ( ind1 = 0, ind2 = 0 )</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">E(f(l1,l2)) = 0</span></div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 100px; width: 1px; height: 1px; overflow: hidden;"><span style="font-size: small;">2^2 * E(f(l1,l2))</span></div>
<p>&nbsp;</p>