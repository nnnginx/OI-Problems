<p>In Shanghai, there are some famous clock towers built more than 100 years ago, such as the office building of Shanghai Customs, Xujiahui Church, etc. Every clock tower��s clock-face consists of three hands: an hour hand, a minute hand, and a second hand. The hands are not move smoothly as time passing. When a second passes, the hands jump to the next place clockwise: the second hand moves 1/60 ring, the minute hand moves 1/3600 ring and the hour hand moves 1/43200 ring.</p>
<p>We assume that every hand��s mass is evenly distributed, and its thickness can be ignored. In other words, every hand��s centre of gravity is at the middle position of the respective hand. Suppose <em>p</em><sub>1</sub>, <em>p</em><sub>2</sub> and <em>p</em><sub>3</sub> are, respectively, the position of the centre of gravity of the hour hand, that of the minute hand, and that of the second hand. The position of all three hands�� centre of gravity, <em>P</em>, is the average of <em>p</em><sub>1</sub>, <em>p</em><sub>2</sub> and <em>p</em><sub>3</sub> weighted by the hands�� mass.</p>
<p>Suppose <em>P</em><sub>1</sub> and <em>P</em><sub>2</sub> are the positions of the three hands�� centre of gravity at the start time and at the end time, respectively. Your task is to calculate the length of the path from <em>P</em><sub>1</sub> to <em>P</em><sub>2</sub>. That is, if <em>P</em><sub>3</sub> is the position of the three hands�� centre of gravity on the clock-face at a point of time between start time and end time, <em>X</em> is the length of the path from <em>P</em><sub>1</sub> to <em>P</em><sub>3</sub>, and <em>Y</em> is the length of the path from <em>P</em><sub>3</sub> to <em>P</em><sub>2</sub>, the length of the path from <em>P</em><sub>1</sub> to <em>P</em><sub>2</sub> is <em>X+Y</em>.</p>
<h3>Input</h3>
<p>Input consists of one or more lines, each line describing one data set. Each line begins with 6 integers: <em>L</em><sub>1</sub>, <em>L</em><sub>2</sub>, <em>L</em><sub>3</sub>, <em>M</em><sub>1</sub>, <em>M</em><sub>2</sub>, <em>M</em><sub>3</sub>, followed by start time and end time. <em>L</em><sub>1</sub>, <em>L</em><sub>2</sub> and <em>L</em><sub>3 </sub>indicate the lengths of hour hand, minute hand and second hand respectively, where 1&lt;= <em>L</em><sub>1</sub>&lt;<em>L</em><sub>2</sub>&lt;<em>L</em><sub>3&nbsp; </sub>&lt;=100. <em>M</em><sub>1</sub>, <em>M</em><sub>2</sub> and <em>M</em><sub>3 </sub>indicate the weights of hour hand, minute hand and second hand respectively, where 1&lt;= <em>M</em><sub>1</sub>, <em>M</em><sub>2</sub>, <em>M</em><sub>3</sub> &lt;=100. The format of start time and end time is <em>hh:mm:ss</em>, where 0&lt;= <em>hh &lt;=</em>23, 0&lt;= <em>mm &lt;=</em>59, and 0&lt;= <em>ss &lt;=</em>59. Start time and end time should be in the same day.</p>
<p>End of input is indicated by a line consisting of -1.</p>
<h3>Output</h3>
<p>For each data set, output a single line. Each line should give the length of the path for the positions of three hands�� centre of gravity<em> </em>at the start time and at the end time. We accept solutions with absolute error less than 10<sup>-2</sup>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1 2 3 1 2 3 00:00:00 00:00:01
3 4 5 1 1 1 09:00:00 18:00:00
-1

<strong>Output:</strong>
0.08
2826.27
</pre>