<p>Dr. Grey is a data analyst, who visualizes various aspects of data received from all over the</p>
<p>world everyday. He is extremely good at sophisticated visualization tools, but yet his favorite is a simple self-made histogram generator.</p>
<p style="text-align: center;"><img src="./24261/file/EQ0hzA3s.png" alt="histogram" width="400" height="298"></p>
<p>Figure 1 is an example of histogram automatically produced by his histogram generator. A histogram is a visual display of frequencies of value occurrences as bars. In this example, values in the interval 0每9 occur five times, those in the interval 10每19 occur three times, and 20每29 and 30每39 once each.</p>
<p>Dr. Grey＊s histogram generator is a simple tool. First, the height of the histogram is fixed, that is, the height of the highest bar is always the same and those of the others are automatically adjusted proportionately. Second, the widths of bars are also fixed. It can only produce a histogram of uniform intervals, that is, each interval of a histogram should have the same width (10 in the above example). Finally, the bar for each interval is painted in a grey color, where the colors of the leftmost and the rightmost intervals are black and white,</p>
<p>respectively, and the darkness of bars monotonically decreases at the same rate from left to right. For instance, in Figure 1, the darkness levels of the four bars are 1, 2/3, 1/3, and 0, respectively.</p>
<p>In this problem, you are requested to estimate ink consumption when printing a histogram on paper. The amount of ink necessary to draw a bar is proportional to both its area and darkness.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The input consists of multiple datasets, each of which contains integers and specifies a value table and intervals for the histogram generator, in the following format:</p>
<p>n w</p>
<p>v1</p>
<p>v2</p>
<p>...</p>
<p>vn</p>
<p>n is the total number of value occurrences for the histogram, and each of the n lines following the first line contains a single value. Note that the same value may possibly occur multiple times.</p>
<p>w is the interval width. A value v is in the first (i.e. leftmost) interval if 0 ≒ v&lt;w, the second one if w ≒ v&lt; 2w, and so on. Note that the interval from 0 (inclusive) to w (exclusive) should be regarded as the leftmost even if no values occur in this interval. The last (i.e. rightmost) interval is the one that includes the largest value in the dataset.</p>
<p>You may assume the following:</p>
<p>1 ≒ n ≒ 100</p>
<p>10 ≒ w ≒ 50</p>
<p>0 ≒ vi ≒ 100 for 1 ≒ i ≒ n</p>
<p>You can also assume that the maximum value is no less than w. This means that the histogram has more than one interval.</p>
<p>The end of the input is indicated by a line containing two zeros.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each dataset, output a line containing the amount of ink consumed in printing the histogram.</p>
<p>One unit of ink is necessary to paint one highest bar black. Assume that 0.01 units of ink per histogram is consumed for various purposes except for painting bars such as drawing lines and characters (see Figure 1). For instance, the amount of ink consumed in printing the histogram in Figure 1 is:</p>
<p style="text-align: center;"><img src="./24261/file/SFiBwkY6.png" alt="example" width="300" height="113"></p>
<p>Each output value should be a 6 decimal fraction.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 50
100
0
100
3 50
100
100
50
10 10
1
2
3
4
5
16
17
18
29
30
0 0

<strong>Output:</strong>
0.510000
0.260000
1.476667<span style="white-space: normal;">
</span></pre>