<p><span style="font-style: italic;">[The original version of this problem (in Spanish) can be found at&nbsp;</span><a style="font-style: italic;" href="http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2012-problems.pdf</a><span style="font-style: italic;">]</span></p>
<p>The International Committee for Professional Chess (ICPC)&nbsp;organizes a Tournament for Advanced Players (TAP) with a very&nbsp;strange methodology. As expected, in each game exactly two&nbsp;players face each other, but in this case only one game takes&nbsp;place at a time, because there is only one chess board&nbsp;available. After receiving the inscriptions for the competitors&nbsp;and assigning them a number, the organization decides&nbsp;arbitrarily what matches are going to take place, and in which&nbsp;order. Each competitor can face any other competitor any number&nbsp;of times, and it is even possible that some competitors never&nbsp;play against others. Once built the general fixture of all the&nbsp;matches to be played, the organization hands each competitor a&nbsp;non-empty list of their rivals, in chronological order (that&nbsp;is, the order in which the matches will take place).</p>
<p>Florencia signed up in first place, so that she was assigned&nbsp;the number <strong>1</strong>. After chatting a bit with the other competitors,&nbsp;she realized that she had lost her list of rivals. Because she&nbsp;does not want to bother the TAP's organizers, she has asked all&nbsp;the other competitors for a copy of their own lists of rivals,&nbsp;hoping that with this information she would be able to&nbsp;reconstruct her lost list. Florencia is not sure if there&nbsp;exists a unique general fixture that is compatible with all the&nbsp;copied lists that she was given by the other competitors.&nbsp;However, she knows that the list that she was given by TAP's&nbsp;organizers is in fact unique. Your task is to help her&nbsp;reconstruct this list.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>Each test case is described using two lines. The first line contains a single integer number <strong>N</strong>, representing the number of&nbsp;competitors (<strong>2&nbsp;</strong><strong>��</strong><strong>&nbsp;N ��&nbsp;9</strong>). Each competitor is identified by a&nbsp;different integer from <strong>1</strong> to <strong>N</strong>, and competitor number <strong>1</strong> is&nbsp;always Florencia. The second line contains <strong>N-1</strong> non-empty&nbsp;strings <strong>L<sub>i</sub></strong> of at most <strong>100</strong> characters each (for <strong>i = 2, 3, ...,&nbsp;N</strong>). The string <strong>L<sub>i</sub></strong> is composed solely of digits between <strong>1</strong> and&nbsp;<strong>N</strong>, excluding digit <strong>i</strong>, and represents the list of rivals of&nbsp;competitor number <strong>i</strong> in chronological order. Note that&nbsp;competitor number <strong>1</strong> appears at least once in one of the given&nbsp;lists. In each test case, there exists a unique list of rivals&nbsp;for competitor number <strong>1</strong> that is compatible with the other lists&nbsp;of rivals. The end of the input is signalled by a line containing the number <strong>-1</strong>.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>For each test case, you should print a single line containing a&nbsp;string, representing the unique list of rivals of competitor&nbsp;number <strong>1</strong> (Florencia) that is compatible with the lists of&nbsp;rivals of the other competitors. The rivals indicated in this&nbsp;list must appear in chronological order.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<span style="font-family: 'courier new', courier;">4
314 142 321
9
31 412 513 614 715 816 917 18
4
11111111111111111111111111111 4 3
-1</span>

<strong>Output:</strong>
<span style="font-family: 'courier new', courier;">324
98765432
22222222222222222222222222222</span><span style="white-space: normal;">
</span></pre>